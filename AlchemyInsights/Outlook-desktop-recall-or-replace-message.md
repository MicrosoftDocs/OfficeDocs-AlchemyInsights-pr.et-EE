---
title: Outlooki töölaua tagasivõtmine või asendamine e-kirja
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496107"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="0c2a5-102">Outlooki e-kirja tagasivõtmine või asendamine</span><span class="sxs-lookup"><span data-stu-id="0c2a5-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="0c2a5-103">Nagu admin, saate **meenutada sõnumeid kasutajate nimel, kasutades PowerShelli**.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="0c2a5-104">Administreerimiskeskusest ei saa sõnumeid meenutada.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="0c2a5-105">Te saate **ainult meenutada sõnumeid, mis saadetakse inimestele teie organisatsioonis**.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="0c2a5-106">Kui sõnum saadeti näiteks Gmaili aadressile, ei saa te seda meenutada.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="0c2a5-107">Võite **meenutada ainult sõnumeid, mis on saadetud Outlook 2016 arvutist**.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="0c2a5-108">Kui kasutaja saadab sõnumi, kasutades Outlook for Mac või Outlook veebis, ei mäleta seda.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="0c2a5-109">E-kirja tagasikutsumiseks või asendamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="0c2a5-110">Valige Outlooki aknast vasakul asuva kaustapaanil kaust saadetud.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="0c2a5-111">Selle avamiseks topeltklõpsake sõnumit, mida soovite meenutada.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="0c2a5-112">Valige vahekaart **sõnum** ja seejärel valige **toimingud** > **seda sõnumit tagasi kutsuda**.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="0c2a5-113">Valige **kustutage selle sõnumi lugemata koopiad** või **kustutage lugemata koopiad ja asendage see uue sõnumiga**ning valige seejärel **OK**.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="0c2a5-114">Kui saadate asendussõnumi, koostage sõnum ja valige siis **saada**.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="0c2a5-115">Sõnumi tagasikutsumise õnnestumine või nurjumine sõltub adressaadi sätetest Outlookis.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="0c2a5-116">Juhised tagasivõtmist kontrollida, vt [käesoleva artikli](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="0c2a5-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="0c2a5-117">Meilisõnumite otsimine ja kustutamine teie organisatsioonis</span><span class="sxs-lookup"><span data-stu-id="0c2a5-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="0c2a5-118">Kui te pole globaalne administraator, tuleb teie konto lisada eDiscovery Manageri rollile või vastavuse otsingu haldamise rollile sõnumite otsimiseks.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="0c2a5-119">Sõnumite kustutamiseks peate liituma organisatsiooni juhtimise rolligrupiga või otsingu ja Purge juhtimise rolliga.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="0c2a5-120">Nende rollide õigused määratakse [turbe-ja Vastavuskeskuses](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="0c2a5-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="0c2a5-121">[Saate luua sisuotsingu](https://docs.microsoft.com/office365/securitycompliance/content-search) , et leida kustutatav sõnum.</span><span class="sxs-lookup"><span data-stu-id="0c2a5-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="0c2a5-122">[Ühendage turbe-ja Vastavuskeskus PowerShelli](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="0c2a5-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="0c2a5-123">Kui kasutate mitme teguriga autentimine, vaadake [ühendust Office 365 turvalisuse ja vastavuse keskus PowerShelli mitme teguriga autentimine abil](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="0c2a5-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>