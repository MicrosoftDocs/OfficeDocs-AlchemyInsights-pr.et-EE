---
title: Tuvasta Kustuta sõnum sündmused auditilogi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508984"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="068bc-102">Auditilogi kustutatud meilisõnumite jaoks</span><span class="sxs-lookup"><span data-stu-id="068bc-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="068bc-103">Alates jaanuarist 2019 Microsoft on sisse lülitada postkasti auditi logimise vaikimisi.</span><span class="sxs-lookup"><span data-stu-id="068bc-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="068bc-104">Vastasel juhul saate mõne kindla kasutaja jaoks kustutada sõnumite kustutamise, peate käsitsi lubama kustutamise toimingute auditeerimine.</span><span class="sxs-lookup"><span data-stu-id="068bc-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="068bc-105">Kui postkasti auditilogi on juba lubatud teie organisatsiooni või konkreetse kasutaja, järgige alltoodud juhiseid.</span><span class="sxs-lookup"><span data-stu-id="068bc-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="068bc-106">Logige sisse [Microsoft 365 Security & vastavuse keskus](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="068bc-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="068bc-107">Klõpsake suvandit **Otsing ja uurimine** ning valige **auditilogi otsing**.</span><span class="sxs-lookup"><span data-stu-id="068bc-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="068bc-108">Saate **valida kuupäevavahemiku alguskuupäeva ja** **lõppkuupäeva** väljadel.</span><span class="sxs-lookup"><span data-stu-id="068bc-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="068bc-109">Määrake kasutaja kasutajanimi, keda soovite uurida (kasutaja, kes kustutas üksused).</span><span class="sxs-lookup"><span data-stu-id="068bc-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="068bc-110">Valige väljal **Tegevused** kustutatud **sõnumid kaustast** kustutatud ja **teisaldati sõnumid kustutatud üksuste kausta**.</span><span class="sxs-lookup"><span data-stu-id="068bc-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="068bc-111">Klõpsake suvandit **Otsing**.</span><span class="sxs-lookup"><span data-stu-id="068bc-111">Click **Search**.</span></span>

<span data-ttu-id="068bc-112">Valige tulemustel auditikirje.</span><span class="sxs-lookup"><span data-stu-id="068bc-112">In the results, select an audit record.</span></span> <span data-ttu-id="068bc-113">Üksikasjade hüpik, klõpsake **rohkem teavet**.</span><span class="sxs-lookup"><span data-stu-id="068bc-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="068bc-114">Välja **Affecteditems** kuvatakse Lisateave kustutatud üksuse kohta (nt teema rida ja üksuse asukoht, kui see kustutati).</span><span class="sxs-lookup"><span data-stu-id="068bc-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="068bc-115">**Clientinfostring** atribuut kuvatakse, kui kustutamine ilmnes Outlookis, Outlook veebis (varem tuntud kui Outlook Web Appi) või mis tahes muu seade.</span><span class="sxs-lookup"><span data-stu-id="068bc-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="068bc-116">Lisateabe saamiseks vaadake määrates, [kes seadistada e-posti suunamine postkasti](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="068bc-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="068bc-117">**Märkus**: kustutatud üksusi ei saa tuua auditilogi funktsiooni abil.</span><span class="sxs-lookup"><span data-stu-id="068bc-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="068bc-118">Kustutatud sõnumite allalaadimiseks Outlookis veebis vaadake teemat [Kustutatud üksuste taastamine rakenduses Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="068bc-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
