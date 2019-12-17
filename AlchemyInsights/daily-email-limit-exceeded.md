---
title: Päevane e-posti piirang on ületatud. Töövoog on peatatud.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053113"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="be48d-103">Päevane e-posti piirang ületatud.</span><span class="sxs-lookup"><span data-stu-id="be48d-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="be48d-104">Töövoog on peatatud.</span><span class="sxs-lookup"><span data-stu-id="be48d-104">Workflow is suspended.</span></span>

<span data-ttu-id="be48d-105">See tõrge võidakse vastu võtta järgmistel juhtudel:</span><span class="sxs-lookup"><span data-stu-id="be48d-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="be48d-106">Teil on töövoo SharePoint Online ' i, mis kasutab SharePoint 2010 või SharePoint 2013 töövoo platvormi tüüp.</span><span class="sxs-lookup"><span data-stu-id="be48d-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="be48d-107">Töövoog on konfigureeritud saatma kohandatud e-kirja rohkem kui 200 kasutajatele korraga, rohkem kui 10 000 adressaadid päevas või rohkem kui 30 sõnumit minutis.</span><span class="sxs-lookup"><span data-stu-id="be48d-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="be48d-108">Töövoo käivitamisel e-kirja ei saadeta ja märkate järgmist käitumist:</span><span class="sxs-lookup"><span data-stu-id="be48d-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="be48d-109">Töövoo abil SharePoint 2013 platvormi tüüp, sirvite **töövoo oleku** lehele.</span><span class="sxs-lookup"><span data-stu-id="be48d-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="be48d-110">Lehel Töövoo olek **sisemine olek** on seatud **käivitatud**ja teave jutumull kuvatakse **ei saa adressaadile saata**.</span><span class="sxs-lookup"><span data-stu-id="be48d-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="be48d-111">Selle probleemi lahendamiseks konfigureerige oma töövoo saata e-kirju, ületamata [Exchange Online ' i saatja piirangud](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="be48d-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="be48d-112">Näiteks kasutage pausi töövoo, saatke e-posti Office 365 rühma, levirühm või e-posti lubatud turberühma või saata sõnumi vähem kui 200 adressaatidele korraga.</span><span class="sxs-lookup"><span data-stu-id="be48d-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="be48d-113">Lisateabe saamiseks lugege järgmist [artiklit](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="be48d-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="be48d-114">Seotud teemad</span><span class="sxs-lookup"><span data-stu-id="be48d-114">Related topics</span></span>
- [<span data-ttu-id="be48d-115">Voo loomine</span><span class="sxs-lookup"><span data-stu-id="be48d-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="be48d-116">SharePointi ja voog</span><span class="sxs-lookup"><span data-stu-id="be48d-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 