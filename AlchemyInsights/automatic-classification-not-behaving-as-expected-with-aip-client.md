---
title: Automaatne klassifikatsioon ei käitudes AIP kliendiga ootuspäraselt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508372"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a><span data-ttu-id="3b32a-102">Automaatne klassifikatsioon ei käitudes AIP kliendiga ootuspäraselt</span><span class="sxs-lookup"><span data-stu-id="3b32a-102">Automatic classification not behaving as expected with the AIP client</span></span>

<span data-ttu-id="3b32a-103">Automaatne klassifikatsioon ei käitudes ootuspäraselt, kasutage järgmisi soovituslikke juhiseid:</span><span class="sxs-lookup"><span data-stu-id="3b32a-103">Automatic classification not behaving as expected, use the following recommended guidelines:</span></span>

1. <span data-ttu-id="3b32a-104">Kui teil on probleeme automaatse märgistamise, vaadake, [Kuidas konfigureerida tingimused automaatne ja soovitatav klassifikatsioon Azure ' i teabekaitse](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="3b32a-104">If you are having issues with automatic labeling, see [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
2. <span data-ttu-id="3b32a-105">Kontrollige, kas kasutate hõlmavaid poliitikaid, mis pole õigesti konfigureeritud: [Kuidas konfigureerida Azure ' i teabe kaitse poliitika teatud kasutajatele, kasutades ulatatud poliitikad](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="3b32a-105">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
3. <span data-ttu-id="3b32a-106">Kui automaatne märgistamine ei tööta Outlooki sildistatud dokumendi ühendamisel, veenduge, et `DRMEncryptProperty` pole määratletud siin kirjeldatud: [IRM registrisätted turvalisuse](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="3b32a-106">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that `DRMEncryptProperty` isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>
4. <span data-ttu-id="3b32a-107">Kui kasutasite oma Azure ' i teabekaitse poliitika [sisseehitatud teabetüüpe](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) , veenduge, et teie sisu vastaks eeldatava vorminguga.</span><span class="sxs-lookup"><span data-stu-id="3b32a-107">If you used the [built-in information types](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) for your Azure Information Protection policy, verify that your content matches the expected format.</span></span>
5. <span data-ttu-id="3b32a-108">Veenduge, et silt oleks sobivalt konfigureeritud **automaatseks** või **soovitatavaks**.</span><span class="sxs-lookup"><span data-stu-id="3b32a-108">Verify that the label is appropriately configured for **Automatic** or **Recommended**.</span></span> <span data-ttu-id="3b32a-109">(**Automaatne** märgistamine on saadaval kõigi Office ' i rakenduste jaoks, samas kui **soovitatav** on kasutada kõiki Office ' i rakendusi peale Outlooki.)</span><span class="sxs-lookup"><span data-stu-id="3b32a-109">(**Automatic** labeling is available for all Office apps, whereas **Recommended** is available for all Office apps except for Outlook.)</span></span>
6. <span data-ttu-id="3b32a-110">Te ei saa kasutada automaatset liigitust dokumentidele ja e-kirjadele, mis olid varem käsitsi märgistatud või varem automaatselt märgistatud kõrgema klassifikatsiooniga.</span><span class="sxs-lookup"><span data-stu-id="3b32a-110">You cannot use automatic classification for documents and emails that were previously manually labeled or previously automatically labeled with a higher classification.</span></span>  <span data-ttu-id="3b32a-111">Lisateabe saamiseks vaadake: [Kuidas rakendatakse automaatselt või soovitatud silte](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).</span><span class="sxs-lookup"><span data-stu-id="3b32a-111">For more information, see: [How automatic or recommended labels are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).</span></span>
7. <span data-ttu-id="3b32a-112">Kui teil on endiselt probleeme, palun koguda Azure ' i teabe kaitse kliendi logid ja kinnitage eksporditud logid oma tugiteenuse pilet.</span><span class="sxs-lookup"><span data-stu-id="3b32a-112">If you are still experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to your support ticket.</span></span> <span data-ttu-id="3b32a-113">Azure ' i teabekaitse logid eksportimiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="3b32a-113">To export Azure Information Protection logs:</span></span>
    - <span data-ttu-id="3b32a-114">Avage Office ' i dokument või looge Outlookis uus e-kiri.</span><span class="sxs-lookup"><span data-stu-id="3b32a-114">Open an Office document or create a new email in Outlook.</span></span>
    - <span data-ttu-id="3b32a-115">Klõpsake valikul **kaitse/tundlikkuse**  >  **Spikker ja tagasiside**.</span><span class="sxs-lookup"><span data-stu-id="3b32a-115">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
    - <span data-ttu-id="3b32a-116">Klikkige käsul **ekspordi logid**.</span><span class="sxs-lookup"><span data-stu-id="3b32a-116">Click **Export Logs**.</span></span>
    - <span data-ttu-id="3b32a-117">Salvestage logid oma asukoha valikule ja kinnitage need oma teenustaotlusele.</span><span class="sxs-lookup"><span data-stu-id="3b32a-117">Save the logs to your choice of location, and attach them to your service request.</span></span>

<span data-ttu-id="3b32a-118">Lisateavet leiate teemast:</span><span class="sxs-lookup"><span data-stu-id="3b32a-118">For additional information, see:</span></span>

- [<span data-ttu-id="3b32a-119">Kuidas konfigureerida automaatse ja soovitatava klassifikatsiooni Azure ' i teabe kaitse tingimused</span><span class="sxs-lookup"><span data-stu-id="3b32a-119">How to configure conditions for automatic and recommended classification for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [<span data-ttu-id="3b32a-120">Kuidas-juhised levinud stsenaariumid, mis kasutavad Azure ' i teabekaitse</span><span class="sxs-lookup"><span data-stu-id="3b32a-120">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [<span data-ttu-id="3b32a-121">Azure ' i teabekaitse dokumentatsiooni läbivaatamine</span><span class="sxs-lookup"><span data-stu-id="3b32a-121">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="3b32a-122">Vaadake üle Azure ' i teabekaitse tellimused ja funktsioonid</span><span class="sxs-lookup"><span data-stu-id="3b32a-122">Review Azure Information Protection subscriptions and features</span></span>](https://azure.microsoft.com/pricing/details/information-protection)
- [<span data-ttu-id="3b32a-123">Azure ' i teabekaitse nõuded</span><span class="sxs-lookup"><span data-stu-id="3b32a-123">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="3b32a-124">Quick Start juhendaja Azure ' i teabekaitse</span><span class="sxs-lookup"><span data-stu-id="3b32a-124">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="3b32a-125">Laadige alla Azure ' i teabekaitse klient</span><span class="sxs-lookup"><span data-stu-id="3b32a-125">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)