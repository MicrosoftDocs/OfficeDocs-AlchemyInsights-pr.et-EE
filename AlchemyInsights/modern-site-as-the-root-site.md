---
title: Kaasaegne saidi juursait
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620755"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="98437-102">Kaasaegne saidi juur</span><span class="sxs-lookup"><span data-stu-id="98437-102">Modern site as root site</span></span>

<span data-ttu-id="98437-103">Oleme hakanud levikuga uus funktsioon, mis võimaldab teil vahetada klassikaline saidi juursait mis kaasaegne veebilehekülg.</span><span class="sxs-lookup"><span data-stu-id="98437-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="98437-104">Vahetada asukoht teise saidiga algse saidi arhiveerimise ajal kasutada [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="98437-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="98437-105">Saadaval Team Site (ühendatud rühma) ja teatise ala.</span><span class="sxs-lookup"><span data-stu-id="98437-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="98437-106">Ärge kustutage oma klassikaline juursait kaasaegsed side saidi loomiseks.</span><span class="sxs-lookup"><span data-stu-id="98437-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="98437-107">See ei toeta Microsoft.</span><span class="sxs-lookup"><span data-stu-id="98437-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="98437-108">Kustutamine juursait teeb kõik SharePointi saidid teie organisatsiooni juurdepääs kõigile kasutajatele, kuni taastamist või luua uue saidi sama URL.</span><span class="sxs-lookup"><span data-stu-id="98437-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="98437-109">Me suhtlemine selle funktsiooni kaudu sõnumikeskus.</span><span class="sxs-lookup"><span data-stu-id="98437-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="98437-110">Teil tuleb arvestada funktsioon olema sisse lülitatud teie rentniku varsti.</span><span class="sxs-lookup"><span data-stu-id="98437-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="98437-111">Tuntud probleemid tootega vahetada saidid</span><span class="sxs-lookup"><span data-stu-id="98437-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="98437-112">Sihtsaidi tagastab "ei leitud" viga (HTTP 404) lühikest aega.</span><span class="sxs-lookup"><span data-stu-id="98437-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="98437-113">Sisu tuleb analüüsitakse uuesti värskendada otsinguregistrisse.</span><span class="sxs-lookup"><span data-stu-id="98437-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="98437-114">Ei mingit käsitsi sammu vajalike, seda tehakse automaatselt.</span><span class="sxs-lookup"><span data-stu-id="98437-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="98437-115">Midagi sõltub "staatiline" lingid (nt faili sünkroonimine ja OneNote) pead käsitsi korrigeerida.</span><span class="sxs-lookup"><span data-stu-id="98437-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="98437-116">Project Serveri saidid võib tekkida vajadus tagada, et need on ikka seotud õigesti kinnitada.</span><span class="sxs-lookup"><span data-stu-id="98437-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
