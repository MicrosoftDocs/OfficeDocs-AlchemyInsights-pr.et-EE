---
title: DLP ei tööta ootuspäraselt
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707806"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="a55a7-102">DLP ei tööta ootuspäraselt</span><span class="sxs-lookup"><span data-stu-id="a55a7-102">DLP not working as expected</span></span>

<span data-ttu-id="a55a7-103">**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="a55a7-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="a55a7-104">**DLP häälestamine**</span><span class="sxs-lookup"><span data-stu-id="a55a7-104">**Setting up DLP**</span></span>

<span data-ttu-id="a55a7-105">Kas teil on probleeme **andmete kaotsimineku vältimise (DLP)** rakenduses Office 365 ei tööta ootuspäraselt?</span><span class="sxs-lookup"><span data-stu-id="a55a7-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="a55a7-106">Kui jah, siis veenduge, et teie **DLP poliitika** oleks õigesti häälestatud ja et teie andmed sisaldavad seda, mida **DLP poliitika** hindamisel otsib.</span><span class="sxs-lookup"><span data-stu-id="a55a7-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="a55a7-107">DLP poliitika abil saate oma ettevõttes tuvastada ja kaitsta tundliku teabe.</span><span class="sxs-lookup"><span data-stu-id="a55a7-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="a55a7-108">DLP poliitikate häälestamiseks kasutage [siin](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)olevat teavet.</span><span class="sxs-lookup"><span data-stu-id="a55a7-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="a55a7-109">**Milliseid DLP poliitikaid otsida?**</span><span class="sxs-lookup"><span data-stu-id="a55a7-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="a55a7-110">Kui kasutate turbe ja ühilduvuse keskustes **sisseehitatud tundliku teabe tüüpe** , leiate DLP poliitikatest nende tundlike tüüpide tuvastamisel kindlad mustrid ja elemendid.</span><span class="sxs-lookup"><span data-stu-id="a55a7-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="a55a7-111">**Sisseehitatud tundlikud teabe tüübid**</span><span class="sxs-lookup"><span data-stu-id="a55a7-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="a55a7-112">Lisateavet sisseehitatud tundlike tüüpide ja selle kohta, mida DLP poliitika otsib tundliku tüübi tuvastamisel, leiate teemast millist tüüpi [tundlikud andmed otsivad](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="a55a7-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="a55a7-113">**Kohandatud tundlikud teabe tüübid**</span><span class="sxs-lookup"><span data-stu-id="a55a7-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="a55a7-114">Kui proovite luua kohandatud tundlikke teabe tüüpe, kasutage kohandatud tundliku tüübi loomise kohta lisateabe saamiseks järgmist artiklit: [kohandatud tundliku teabe tüübi loomine](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="a55a7-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="a55a7-115">**DLP poliitika testimine**</span><span class="sxs-lookup"><span data-stu-id="a55a7-115">**Test a DLP policy**</span></span>

<span data-ttu-id="a55a7-116">Kui soovite testida andmeid sisseehitatud või kohandatud tundliku teabe tüübiga, kasutage jaotises **klassifikatsioonid** tundlikud teabe tüübid suvandit **testi tüüp**  >  .</span><span class="sxs-lookup"><span data-stu-id="a55a7-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="a55a7-117">Lisateavet leiate teemast [kohandatud tundliku teabe tüüpide testimine](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="a55a7-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="a55a7-118">**Aruanded**</span><span class="sxs-lookup"><span data-stu-id="a55a7-118">**Reports**</span></span>
  
- <span data-ttu-id="a55a7-119">Delikaatsete andmete ülevaadete hankimine [DLP aruannetega.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="a55a7-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="a55a7-120">Vaadake sündmuse konkreetseid üksikasju [intsidendi](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)kohta.</span><span class="sxs-lookup"><span data-stu-id="a55a7-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
