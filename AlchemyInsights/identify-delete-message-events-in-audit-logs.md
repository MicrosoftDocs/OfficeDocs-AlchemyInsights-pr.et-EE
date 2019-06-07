---
title: Kustuta sõnum sündmused auditilogid tuvastada
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 0fb5d6aa0c99f7f68459c40302869bed69583b3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755149"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="56151-102">Auditilogide kustutatud e-kirju</span><span class="sxs-lookup"><span data-stu-id="56151-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="56151-103">Alates jaanuarist 2019, Microsoft lülitab Postkasti auditilogi vaikimisi.</span><span class="sxs-lookup"><span data-stu-id="56151-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="56151-104">Muul juhul vaadata Kustuta sõnum sündmused kindla kasutaja, peate käsitsi lubada auditeerimiseks toimingu delete.</span><span class="sxs-lookup"><span data-stu-id="56151-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="56151-105">Kui postkasti auditi logimine on lubatud juba teie organisatsiooni jaoks või konkreetse kasutaja, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="56151-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="56151-106">Logige sisse [Office 365 & vastavuse Turvakeskus](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="56151-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="56151-107">Valige **Auditi logifaili Otsi**nuppu **Otsi ja uurimine** .</span><span class="sxs-lookup"><span data-stu-id="56151-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="56151-108">Valige kuupäevavahemik väljadele **Alguskuupäev** ja **lõppkuupäev** .</span><span class="sxs-lookup"><span data-stu-id="56151-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="56151-109">Määrake kasutajanimi kasutaja, mida soovite uurida (kasutaja kustutatud üksused).</span><span class="sxs-lookup"><span data-stu-id="56151-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="56151-110">Valige väljal **tegevuse** **kustutatud sõnumite kausta Kustutatud** ja **Moved sõnumite kausta Kustutatud**.</span><span class="sxs-lookup"><span data-stu-id="56151-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="56151-111">Klõpsake nuppu **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="56151-111">Click **Search**.</span></span>

<span data-ttu-id="56151-112">Tulemused, valige audit kirje.</span><span class="sxs-lookup"><span data-stu-id="56151-112">In the results, select an audit record.</span></span> <span data-ttu-id="56151-113">Hüpik üksikasjad nuppu **Lisateave**.</span><span class="sxs-lookup"><span data-stu-id="56151-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="56151-114">Lisateavet kustutatud üksusi (nt teema ja kui see on kustutatud üksuse asukoht) kuvatakse väljal **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="56151-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="56151-115">**ClientInfoString** vara näitab kui kustutamise toimunud Outlooki, Outlook web (varasema nimega Outlook Web App) või teiste seadmetega.</span><span class="sxs-lookup"><span data-stu-id="56151-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="56151-116">Lisateabe saamiseks vt [Determining kes seadistada e-posti edasisuunamise postkasti](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="56151-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="56151-117">**Märkus**: te ei saa tuua auditi logifaili funktsiooniga kustutatud üksuste.</span><span class="sxs-lookup"><span data-stu-id="56151-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="56151-118">Taastada kustutatud üksused Outlook veebis, Vaata [taastada kustutatud üksused Outlook Web Appis](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="56151-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
