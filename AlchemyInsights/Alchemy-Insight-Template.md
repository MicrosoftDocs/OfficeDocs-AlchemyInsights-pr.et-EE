---
title: sama faili nimi on parim
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 37398436435fb72cb5c8dca2d0798b86a0c8ccc9
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30762061"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="7e213-102">Nõutav alkeemia päise H1, H2's ei tööta.</span><span class="sxs-lookup"><span data-stu-id="7e213-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="7e213-103">Heade tavade ja suuniste alkeemia authoring:</span><span class="sxs-lookup"><span data-stu-id="7e213-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="7e213-104">**Pesa alkeemia ülevaatlikke kaustad**- see rikub URL-i struktuuri.</span><span class="sxs-lookup"><span data-stu-id="7e213-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="7e213-105">Ootame, millega seda arvesse.</span><span class="sxs-lookup"><span data-stu-id="7e213-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="7e213-106">Failid kaustas **AlchemyInsights** peaks olema väike failinimesid ruumid ex sidekriipsudega.</span><span class="sxs-lookup"><span data-stu-id="7e213-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="7e213-107">***Kuidas-to-luba-otsuse-ootel***.</span><span class="sxs-lookup"><span data-stu-id="7e213-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="7e213-108">Reegli ID või ämber ID: [alkeemia partneriportaal](https://alchemyportal.azurewebsites.net) kaasata ms.custom välja.</span><span class="sxs-lookup"><span data-stu-id="7e213-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="7e213-109">ex.</span><span class="sxs-lookup"><span data-stu-id="7e213-109">ex.</span></span> <span data-ttu-id="7e213-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="7e213-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="7e213-111">Kasutada ülejäänud metaandmete faili ülaosas malli.</span><span class="sxs-lookup"><span data-stu-id="7e213-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="7e213-112">[Portaal alkeemia Partner](https://alchemyportal.azurewebsites.net)navigeerida jaotiseni **kliendile ülevaate pealkiri:** ja kasutamine, et kohe alguses tuleb seadusandjal punkti oma H1 pealkiri tutvustus.</span><span class="sxs-lookup"><span data-stu-id="7e213-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="7e213-113">Alkeemia teadmisi peab olema ainult ühe H1 ülaosas või vaheaega tootmises.</span><span class="sxs-lookup"><span data-stu-id="7e213-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="7e213-114">H2s ei muuda nii kasutada **paksu** või teiste konventsioonidega tähenda eraldi.</span><span class="sxs-lookup"><span data-stu-id="7e213-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="7e213-115">Seejärel sisestage kasutades eelnõu materjali alkeemia reegel lehe jaotises klientide vaatenurki kehatekst</span><span class="sxs-lookup"><span data-stu-id="7e213-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="7e213-116">Täppidega on ilusad</span><span class="sxs-lookup"><span data-stu-id="7e213-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="7e213-117">Nummerdatud loendite liiga</span><span class="sxs-lookup"><span data-stu-id="7e213-117">Numbered lists too</span></span>
    1. <span data-ttu-id="7e213-118">**Rasvase** ja *kursiivkirja* on a-ok</span><span class="sxs-lookup"><span data-stu-id="7e213-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="7e213-119">Lingid tuleb alati kas **"web linke" / väline** või **sügav-viited Kasutajaliidese elemendid**, mitte sisemised lingid.</span><span class="sxs-lookup"><span data-stu-id="7e213-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="7e213-120">Pildid ei toeta praegu, kuid see on peal.</span><span class="sxs-lookup"><span data-stu-id="7e213-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="7e213-121">Ja see on tõesti juba natuke liiga pikk.</span><span class="sxs-lookup"><span data-stu-id="7e213-121">And this is really already a bit too long.</span></span> <span data-ttu-id="7e213-122">On umbes 400 tähemärki---</span><span class="sxs-lookup"><span data-stu-id="7e213-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="7e213-123">Kui teie sisu on valmis, tõmmake see live kontorisse.</span><span class="sxs-lookup"><span data-stu-id="7e213-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="7e213-124">Seejärel minge [alkeemia partneriportaal](https://alchemyportal.azurewebsites.net) ja sisestage faili nimi väljale.</span><span class="sxs-lookup"><span data-stu-id="7e213-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="7e213-125">M</span><span class="sxs-lookup"><span data-stu-id="7e213-125">M</span></span>