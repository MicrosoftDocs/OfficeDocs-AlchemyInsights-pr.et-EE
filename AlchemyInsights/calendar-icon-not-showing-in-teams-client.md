---
title: Kalendri ikooni ei kuvata Teamsi klientrakenduses
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819949"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="19fe6-102">Kalendri ikooni ei kuvata Teamsi klientrakenduses</span><span class="sxs-lookup"><span data-stu-id="19fe6-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="19fe6-103">Teamsi vahekaart Kalender vajab Exchange’i veebiteenuste kaudu juurdepääsu Exchange’i postkastile.</span><span class="sxs-lookup"><span data-stu-id="19fe6-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="19fe6-104">Exchange’i postkast võib olla veebipõhine või kohapealne.</span><span class="sxs-lookup"><span data-stu-id="19fe6-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="19fe6-105">Veebiversiooni kasutajate puhul, kes vahekaarti Kalender ei näe, veenduge, et neil [oleks Exchange Online’i postkasti litsents ja postkast oleks lubatud](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="19fe6-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="19fe6-106">Kui kasutajal on Exchange Online’is kehtiv postkast, kuid nad endiselt vahekaarti Kalender ei näe, võib teil olla probleem võrguga.</span><span class="sxs-lookup"><span data-stu-id="19fe6-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="19fe6-107">Kasutage [Microsofti kaugühenduvuse analüsaatorit](https://testconnectivity.microsoft.com/) ja käitage mõjutatud kasutaja jaoks **Microsoft Exchange’i veebiteenuste ühenduvuse testid**.</span><span class="sxs-lookup"><span data-stu-id="19fe6-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="19fe6-108">Lõpuks kontrollige [Teamsi rakenduste rakenduse häälestuspoliitikaid](https://admin.teams.microsoft.com/policies/app-setup), et tagada, et rakendus Kalender ei oleks kasutajale rakendatavast poliitikast eemaldatud (kõige tõenäolisemalt **globaalne (vaikimisi organisatsiooniülene)**.</span><span class="sxs-lookup"><span data-stu-id="19fe6-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="19fe6-109">Kui teie kasutajad on majutatud kohapeal, peate kinnitama, et teie hübriidkonfiguratsiooni seisund oleks hea.</span><span class="sxs-lookup"><span data-stu-id="19fe6-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="19fe6-110">Kasutage tõrkeotsinguks [hübriidkonfiguratsiooni viisardit](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="19fe6-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="19fe6-111">Pange tähele, et [Teamsi jaoks on vajalik Exchange 2016 CU3 või kõrgem](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="19fe6-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
