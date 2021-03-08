---
title: Oma asutuse meilisõnumite otsimine ja kustutamine
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524280"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="35578-102">Oma asutuse meilisõnumite otsimine ja kustutamine</span><span class="sxs-lookup"><span data-stu-id="35578-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="35578-103">Tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="35578-103">Follow these steps:</span></span>

1. <span data-ttu-id="35578-104">Kui te pole üldadministraator, saate sõnumite otsimiseks lisada oma konto e- **juurdluse halduri rollirühma** või **vastavuse otsingu juhtimise rollile**.</span><span class="sxs-lookup"><span data-stu-id="35578-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="35578-105">Sõnumite kustutamiseks peate liituma **organisatsiooni juhtimise rollirühma** või **otsingu ja likvideerimise rolliga**.</span><span class="sxs-lookup"><span data-stu-id="35578-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="35578-106">Nende rollide kasutusõigused määratakse [turbe & täitmise keskuses.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="35578-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="35578-107">[Saate luua sisu otsimise](https://docs.microsoft.com/office365/securitycompliance/content-search) , et leida sõnum, mille soovite kustutada.</span><span class="sxs-lookup"><span data-stu-id="35578-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="35578-108">[Looge ühendus turbe & vastavuse keskusega PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="35578-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="35578-109">Kui kasutate MFA-i, lugege järgmisi juhiseid: [ühenduse loomine turbe & ühilduvuse keskusega PowerShelli abil mitme teguriga autentimine](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="35578-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="35578-110">Kustutage sõnum: Käivitage `New-ComplianceSearchAction` cmdlet-käsk, et sõnum kustutada.</span><span class="sxs-lookup"><span data-stu-id="35578-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="35578-111">Kustutatud sõnumid teisaldatakse kasutaja taastatavate üksuste kausta.</span><span class="sxs-lookup"><span data-stu-id="35578-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="35578-112">Näites toodud juhised leiate artiklist [3: sõnumi kustutamine.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="35578-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
