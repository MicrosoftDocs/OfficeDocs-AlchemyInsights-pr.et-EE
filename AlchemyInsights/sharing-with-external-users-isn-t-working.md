---
title: Ühiskasutus väliste kasutajatega ei tööta
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912998"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="e66c5-102">SharePointi sisu ühiskasutuse probleemide lahendamine väliste kasutajatega</span><span class="sxs-lookup"><span data-stu-id="e66c5-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="e66c5-103">Veenduge, et väline ühiskasutus oleks teie organisatsiooni jaoks sisse lülitatud.</span><span class="sxs-lookup"><span data-stu-id="e66c5-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="e66c5-104">[microsofti 365 halduskeskus lehele teenuste &amp; lisandmoodulid](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ja klõpsake **saite**.</span><span class="sxs-lookup"><span data-stu-id="e66c5-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="e66c5-105">Veenduge, et säte oleks sisse lülitatud.</span><span class="sxs-lookup"><span data-stu-id="e66c5-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="e66c5-106">Kui "ainult olemasolevad välised kasutajad" on valitud, veenduge, et väline kasutaja on loetletud Microsoft 365 halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="e66c5-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="e66c5-107">Veenduge, et väline ühiskasutus oleks saidi jaoks sisse lülitatud.</span><span class="sxs-lookup"><span data-stu-id="e66c5-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="e66c5-108">Klassikaline saidikogumi:</span><span class="sxs-lookup"><span data-stu-id="e66c5-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="e66c5-109">Klõpsake uue SharePointi administreerimiskeskus vasakpoolsel paanil **saidid**.</span><span class="sxs-lookup"><span data-stu-id="e66c5-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="e66c5-110">Valige sait või saidid ja klõpsake lindil valikul **ühiskasutus**.</span><span class="sxs-lookup"><span data-stu-id="e66c5-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="e66c5-111">Meeskonnatöö sait, mis kuulub Microsoft 365 rühma või side saidi:</span><span class="sxs-lookup"><span data-stu-id="e66c5-111">For a team site that belongs to an Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="e66c5-112">Need uued saiditüübid on sama ühiskasutuse säte kui teie organisatsiooni hõlmav säte, kui organisatsiooni hõlmav säte võimaldab failide ühiskasutust, kasutades linke, mis ei nõua sisselogimist.</span><span class="sxs-lookup"><span data-stu-id="e66c5-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="e66c5-113">Sel juhul saidid võimaldavad ühiskasutus uute ja olemasolevate väliste kasutajatega, kes sisse logida.</span><span class="sxs-lookup"><span data-stu-id="e66c5-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="e66c5-114">Kindlate saitide sätte muutmiseks kasutage uut SharePointi administreerimiskeskust või PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="e66c5-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="e66c5-115">[Lisateave](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="e66c5-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="e66c5-116">Väline ühiskasutuse säte iga saidi jaoks võib olla kitsendavam kui teie organisatsiooni hõlmav säte, kuid mitte rohkem kui organisatsiooni hõlmav säte.</span><span class="sxs-lookup"><span data-stu-id="e66c5-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

