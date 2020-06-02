---
title: DLP reegel krediitkaardi number ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507402"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="dbe6b-102">DLP probleemid krediitkaardi numbrid</span><span class="sxs-lookup"><span data-stu-id="dbe6b-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="dbe6b-103">**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="dbe6b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="dbe6b-104">**DLP probleemid krediitkaardi numbrid**</span><span class="sxs-lookup"><span data-stu-id="dbe6b-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="dbe6b-105">Kas teil on probleeme **andmete kadu vältimine (DLP)** ei tööta sisu, mis sisaldab **krediitkaardi number** , kasutades DLP tundliku teabe tüüp O365?</span><span class="sxs-lookup"><span data-stu-id="dbe6b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="dbe6b-106">Kui jah, veenduge, et teie sisu sisaldab vajalikku teavet, et käivitada DLP poliitika, kui see on hinnatud.</span><span class="sxs-lookup"><span data-stu-id="dbe6b-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="dbe6b-107">Näiteks **krediitkaardi poliitika** konfigureeritud usalduse tase 85%, hinnatakse ja tuleb tuvastada reegli käivitamiseks:</span><span class="sxs-lookup"><span data-stu-id="dbe6b-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="dbe6b-108">**[Formaat:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 numbrit, mida saab vormindada või vormindamata (dddddddddddddddd) ja peab läbima Luhn test.</span><span class="sxs-lookup"><span data-stu-id="dbe6b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="dbe6b-109">**[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Väga keeruline ja jõuline muster, mis tuvastab kaarte kõigi suuremate kaubamärkide kogu maailmas, sealhulgas Visa, MasterCard, Discover kaart, JCB, American Express, kinkekaardid, ja söökla kaardid.</span><span class="sxs-lookup"><span data-stu-id="dbe6b-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="dbe6b-110">**[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Jah, Luhn-i kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="dbe6b-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="dbe6b-111">**[Määratlus:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP poliitika on 85% kindel, et see on avastatud seda tüüpi tundlik teave, kui lähedus 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="dbe6b-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="dbe6b-112">Funktsioon Func_credit_card otsib sisu, mis vastab mustrile.</span><span class="sxs-lookup"><span data-stu-id="dbe6b-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="dbe6b-113">Üks järgmistest on täidetud:</span><span class="sxs-lookup"><span data-stu-id="dbe6b-113">One of the following is true:</span></span>

  - <span data-ttu-id="dbe6b-114">Leitakse märksõna Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="dbe6b-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="dbe6b-115">Leitakse märksõna Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="dbe6b-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="dbe6b-116">Funktsioon Func_expiration_date otsib kuupäeva paremas kuupäevavormingus.</span><span class="sxs-lookup"><span data-stu-id="dbe6b-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="dbe6b-117">Kontrollsumma möödub</span><span class="sxs-lookup"><span data-stu-id="dbe6b-117">The checksum passes</span></span>

    <span data-ttu-id="dbe6b-118">Näiteks järgmine näidis käivitab DLP krediitkaardi number poliitika:</span><span class="sxs-lookup"><span data-stu-id="dbe6b-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="dbe6b-119">Viisa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="dbe6b-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="dbe6b-120">Aegub: 2/2009</span><span class="sxs-lookup"><span data-stu-id="dbe6b-120">Expires: 2/2009</span></span>

<span data-ttu-id="dbe6b-121">Lisateabe saamiseks selle kohta, mida on vaja teie sisu tuvastada **krediitkaardi number** , lugege järgmist jaotist selles artiklis: [mida tundliku teabe tüübid otsida krediitkaardi #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="dbe6b-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="dbe6b-122">Kasutades muu sisseehitatud tundliku teabe tüüp, lugege järgmist artiklit teavet, mida on vaja muud tüüpi: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="dbe6b-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  