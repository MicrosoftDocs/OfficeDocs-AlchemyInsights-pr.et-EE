---
title: Setup DKIM Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765011"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="739fc-102">Setup DKIM Office 365</span><span class="sxs-lookup"><span data-stu-id="739fc-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="739fc-103">Täielikud juhised konfigureerimiseks DKIM kohandatud domeenide Office 365 on [siin](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="739fc-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="739fc-104">**Iga** kohandatud domeeni, peate looma **kaks** DKIM CNAME-kirjeid, teie domeeni DNS-i hostimisteenuses (tavaliselt domeeniregistraatori).</span><span class="sxs-lookup"><span data-stu-id="739fc-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="739fc-105">Nt contoso.com ja fourthcoffee.com nõuavad neli DKIM CNAME-kirjeid: kaks contoso.com ja kaks fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="739fc-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="739fc-106">**Iga** kohandatud domeeni DKIM CNAME-kirjeid kasutada järgmisi vorminguid:</span><span class="sxs-lookup"><span data-stu-id="739fc-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="739fc-107">**Serveri nimi**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="739fc-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="739fc-108">**Aadress või väärtus viitab**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="739fc-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="739fc-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="739fc-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="739fc-110">**Serveri nimi**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="739fc-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="739fc-111">**Aadress või väärtus viitab**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="739fc-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="739fc-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="739fc-112">**TTL**: 3600</span></span>

   <span data-ttu-id="739fc-113">\<DomainGUID\> on tekst vasakul `.mail.protection.outlook.com` MX-kirjes kohandatud kohandatud domeeni (nt `contoso-com` jaoks domeeni contoso.com).</span><span class="sxs-lookup"><span data-stu-id="739fc-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="739fc-114">\<InitialDomain\> on domeen, kui olete registreerunud Office 365 (nt contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="739fc-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="739fc-115">Pärast loomist kohandatud domeenide CNAME-kirjeid, täitke järgmised juhised:</span><span class="sxs-lookup"><span data-stu-id="739fc-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="739fc-116">saanud.</span><span class="sxs-lookup"><span data-stu-id="739fc-116">a.</span></span> <span data-ttu-id="739fc-117">[Office 365 sisselogimine](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) töö- või koolikontoga kontoga.</span><span class="sxs-lookup"><span data-stu-id="739fc-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="739fc-118">b.</span><span class="sxs-lookup"><span data-stu-id="739fc-118">b.</span></span> <span data-ttu-id="739fc-119">Valige rakenduse käivitaja ikoon ülemises vasakus ja **Admin**.</span><span class="sxs-lookup"><span data-stu-id="739fc-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="739fc-120">c.</span><span class="sxs-lookup"><span data-stu-id="739fc-120">c.</span></span> <span data-ttu-id="739fc-121">Vasakus navigation, laiendada **Admin** ja valige **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="739fc-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="739fc-122">d.</span><span class="sxs-lookup"><span data-stu-id="739fc-122">d.</span></span> <span data-ttu-id="739fc-123">Mine **kaitse** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="739fc-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="739fc-124">e.</span><span class="sxs-lookup"><span data-stu-id="739fc-124">e.</span></span> <span data-ttu-id="739fc-125">Valige domeeni ja valige **lubade kasutada programmi** **Logi**sõnumeid selle domeeni DKIM allkirjad.</span><span class="sxs-lookup"><span data-stu-id="739fc-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="739fc-126">Korrake seda toimingut iga kohandatud domeeni.</span><span class="sxs-lookup"><span data-stu-id="739fc-126">Repeat this step for each custom domain.</span></span>
