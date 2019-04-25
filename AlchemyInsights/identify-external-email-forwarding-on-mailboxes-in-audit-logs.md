---
title: Tuvastada postkasti auditilogide väline e-posti saatmise
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417208"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="34f3f-102">Tuvastada välise Meili edasisaatmine on konfigureeritud postkastide</span><span class="sxs-lookup"><span data-stu-id="34f3f-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="34f3f-103">Kui kasutaja konfigureerib väliste meilide edasisaatmise funktsiooni postkast, auditeerib tegevuse osana cmdleti **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="34f3f-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="34f3f-104">Kuvatakse tegevuse turvalisuse & vastavuse Center auditi logifaili otsingu abil.</span><span class="sxs-lookup"><span data-stu-id="34f3f-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="34f3f-105">Logige sisse [Office 365 & vastavuse Turvakeskus](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="34f3f-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="34f3f-106">Valige **Auditi logifaili Otsi**nuppu **Otsi ja uurimine** .</span><span class="sxs-lookup"><span data-stu-id="34f3f-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="34f3f-107">Valige kuupäevavahemik väljadele **Alguskuupäev** ja **lõppkuupäev** .</span><span class="sxs-lookup"><span data-stu-id="34f3f-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="34f3f-108">Te ei pea määrama kasutajanime.</span><span class="sxs-lookup"><span data-stu-id="34f3f-108">You don't need to specify a username.</span></span> <span data-ttu-id="34f3f-109">Veenduge **tegevuse** välja näidata **kõigi tegevuste tulemusi**.</span><span class="sxs-lookup"><span data-stu-id="34f3f-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="34f3f-110">Klõpsake nuppu **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="34f3f-110">Click **Search**.</span></span>

<span data-ttu-id="34f3f-111">Tulemites klõpsake **Filtri tulemused** ja tippige **Set-Mailbox** väljale tegevuse filter.</span><span class="sxs-lookup"><span data-stu-id="34f3f-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="34f3f-112">Valige kirjega auditi tulemused.</span><span class="sxs-lookup"><span data-stu-id="34f3f-112">Select an audit record in the results.</span></span> <span data-ttu-id="34f3f-113">Hüpik **üksikasjad** klõpsake **Lisateabe saamiseks**.</span><span class="sxs-lookup"><span data-stu-id="34f3f-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="34f3f-114">Sa pead vaatama iga auditikirje kindlaks, kas tegevus on seotud e-posti edastamise üksikasjad.</span><span class="sxs-lookup"><span data-stu-id="34f3f-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="34f3f-115">**ObjectId väärtuse**: alias väärtuse muutmise postkasti.</span><span class="sxs-lookup"><span data-stu-id="34f3f-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="34f3f-116">**Parameetrid**: _ForwardingSmtpAddress_ näitab target e-posti aadress.</span><span class="sxs-lookup"><span data-stu-id="34f3f-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="34f3f-117">**Kasutajanimi**: kasutaja konfigureeritud Meili edasisaatmine **ObjectId väärtuse** väljal postkastis.</span><span class="sxs-lookup"><span data-stu-id="34f3f-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="34f3f-118">Lisateabe saamiseks vt [Determining kes seadistada e-posti edasisuunamise postkasti](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="34f3f-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
