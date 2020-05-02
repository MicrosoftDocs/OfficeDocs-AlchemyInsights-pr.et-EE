---
title: Mikro viivitused või ahendamine Exchange Online PowerShellis
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947833"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="e6ad1-102">Mikro viivitused või ahendamine Exchange Online PowerShellis</span><span class="sxs-lookup"><span data-stu-id="e6ad1-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="e6ad1-103">Exchange Online’is skriptide ja cmdlet-käskude käitamisel võite näha hoiatusi „Mikro viivitus rakendatud“ või viivitusi.</span><span class="sxs-lookup"><span data-stu-id="e6ad1-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="e6ad1-104">Järgnevalt on toodud sellega seoses kaks soovitust.</span><span class="sxs-lookup"><span data-stu-id="e6ad1-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="e6ad1-105">Võite proovida kasutada [Exchange Online’i versiooni 2 PowerShelli moodulit](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), mis sisaldab cmdlet-käske, mis põhinevad REST API-l ja mida teostatakse olulised rohkem.</span><span class="sxs-lookup"><span data-stu-id="e6ad1-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="e6ad1-106">See võib olla suurepärane lahendus paljudele cmdleti hankimise käskude, mida sageli kasutatakse.</span><span class="sxs-lookup"><span data-stu-id="e6ad1-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="e6ad1-107">Kui peate kasutama cmdlet-käske, mis ei ole versiooni 2 moodulis veel kaetud, vaadake teemat [PowerShelli cmdlet-käskude käitamine paljudele Office 365 kasutajatele](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), mis selgitab, kuidas navigeerida oodatud PowerShelli ahendamise piirangutes Exchange Online’is.</span><span class="sxs-lookup"><span data-stu-id="e6ad1-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>