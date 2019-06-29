---
title: 1491-Search-Not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355873"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="1c8aa-102">Otsing ei tagasta oodatavad tulemused</span><span class="sxs-lookup"><span data-stu-id="1c8aa-102">Content Search not returning expected results</span></span>

<span data-ttu-id="1c8aa-103">Sõites sisu otsingud: Office 365 turvalisus & vastavuse Center, saate ootamatu Otsingu tulemused.</span><span class="sxs-lookup"><span data-stu-id="1c8aa-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="1c8aa-104">Kaaluge järgmist asjad, mis võib mõjutada teie otsingu tulemused:</span><span class="sxs-lookup"><span data-stu-id="1c8aa-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="1c8aa-105">**Sisu kohtades ja Otsi tingimustes**: Veenduge, et valitud sisu ettenähtud kohas ja otsingu tingimused.</span><span class="sxs-lookup"><span data-stu-id="1c8aa-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="1c8aa-106">Kui käivitasite annab suur otsing (paljudes kohtades), kaaluda mitmeks mitu otsinguid.</span><span class="sxs-lookup"><span data-stu-id="1c8aa-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="1c8aa-107">**Osaliselt indekseeritud üksuste**: [osaliselt indekseeritud üksuste](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) postkastidest sisalduvad hinnanguline Otsingu tulemused.</span><span class="sxs-lookup"><span data-stu-id="1c8aa-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="1c8aa-108">Siiski osaliselt indekseeritud üksuste SharePointis või OneDrive saidid pole lisatud Otsi hinnang.</span><span class="sxs-lookup"><span data-stu-id="1c8aa-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="1c8aa-109">**Otsi vead**: palju postkaste (üle 100 000 postkastid) otsimisel võite saada Otsi tõrkeid, tõrkekoodide nagu CS008-009 ja CS012-002).</span><span class="sxs-lookup"><span data-stu-id="1c8aa-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="1c8aa-110">Sel juhul proovige uuesti otsida ainult ebaõnnestunud sisu asukohad.</span><span class="sxs-lookup"><span data-stu-id="1c8aa-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="1c8aa-111">Vaata [see artikkel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) rohkem teavet.</span><span class="sxs-lookup"><span data-stu-id="1c8aa-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
