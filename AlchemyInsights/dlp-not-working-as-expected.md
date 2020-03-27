---
title: DLP ei tööta ootuspäraselt
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977434"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="501ea-102">DLP ei tööta ootuspäraselt</span><span class="sxs-lookup"><span data-stu-id="501ea-102">DLP not working as expected</span></span>

<span data-ttu-id="501ea-103">**Oluline**: nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadavad-Palun külastage [SharePoint Online ajutised funktsiooni kohandused](https://aka.ms/ODSPAdjustments) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="501ea-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="501ea-104">**DLP seadistamine**</span><span class="sxs-lookup"><span data-stu-id="501ea-104">**Setting up DLP**</span></span>

<span data-ttu-id="501ea-105">Kas teil on probleeme **andmete kadu vältimine (DLP)** Office 365 ei tööta ootuspäraselt?</span><span class="sxs-lookup"><span data-stu-id="501ea-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="501ea-106">Kui jah, veenduge, et teie **DLP poliitika** on õigesti seadistatud ja et teie andmed sisaldavad seda, mida **DLP poliitika** otsib, kui seda hinnatakse.</span><span class="sxs-lookup"><span data-stu-id="501ea-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="501ea-107">DLP poliitika võimaldab teil tuvastada ja kaitsta tundliku loomuga teavet oma organisatsioonis.</span><span class="sxs-lookup"><span data-stu-id="501ea-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="501ea-108">DLP poliitikate häälestamise puhul kasutage [siin](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)olevat teavet.</span><span class="sxs-lookup"><span data-stu-id="501ea-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="501ea-109">**Mida DLP poliitikad otsida**</span><span class="sxs-lookup"><span data-stu-id="501ea-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="501ea-110">**Sisseehitatud tundliku teabe tüüpide** kasutamisel Office 365 turvalisuse ja vastavuse keskus, DLP poliitika otsida konkreetseid mustreid ja elemente, kui need tundlikud tüübid tuvastada.</span><span class="sxs-lookup"><span data-stu-id="501ea-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="501ea-111">**Sisseehitatud tundlikud teabetüübid**</span><span class="sxs-lookup"><span data-stu-id="501ea-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="501ea-112">Teave sisseehitatud tundlik tüübid ja mida DLP poliitika otsib kui tuvastamine tundlik tüüp, vaadake: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="501ea-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="501ea-113">**Kohandatud tundliku teabe tüübid**</span><span class="sxs-lookup"><span data-stu-id="501ea-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="501ea-114">Kui proovite luua kohandatud tundliku teabe tüüpe, kasutage järgmist artiklit teabe saamiseks kohandatud tundliku tüübi loomise kohta: [kohandatud tundliku teabe tüübi loomine](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="501ea-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="501ea-115">**DLP poliitika testimine**</span><span class="sxs-lookup"><span data-stu-id="501ea-115">**Test a DLP policy**</span></span>

<span data-ttu-id="501ea-116">Oma andmete testimiseks sisseehitatud või kohandatud tundliku teabe tüübiga kasutage suvandit **testi tüüp jaotises liigitustundlikud** **Classifications** > **teabetüübid**.</span><span class="sxs-lookup"><span data-stu-id="501ea-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="501ea-117">Lisateabe saamiseks vt teemat [kohandatud tundliku teabe tüüpide testimine](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="501ea-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="501ea-118">**Aruanded**</span><span class="sxs-lookup"><span data-stu-id="501ea-118">**Reports**</span></span>
  
- <span data-ttu-id="501ea-119">Hankige tundlikud andmete ülevaated [DLP aruannetega.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="501ea-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="501ea-120">Vaadake juhtumi konkreetseid üksikasju [intsidendi aruandega](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="501ea-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
