---
title: Määrata 0x8004de40 viga OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525055"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="82ad5-102">Määrata 0x8004de40 viga OneDrive</span><span class="sxs-lookup"><span data-stu-id="82ad5-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="82ad5-103">Kui saate tõrketeate 0x8004de40 OneDrive:</span><span class="sxs-lookup"><span data-stu-id="82ad5-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="82ad5-104">Kui teie Acitve Directory domeeni mõjutatud arvuti taaskäivitama.</span><span class="sxs-lookup"><span data-stu-id="82ad5-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="82ad5-105">Kui reboot ei lahenda probleemi, unjoin ja ühineks Azure AD seadmesse.</span><span class="sxs-lookup"><span data-stu-id="82ad5-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="82ad5-106">**Märkus**: te peate olema ettevõtte võrgus nende teostamisel.</span><span class="sxs-lookup"><span data-stu-id="82ad5-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="82ad5-107">Ei täida järgmiselt, kui te ei ole võimalik luua ühendus oma ettevõtte infrastruktuuri (näiteks reisides).</span><span class="sxs-lookup"><span data-stu-id="82ad5-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="82ad5-108">Avage administraatoriõigustes Käsuviip.</span><span class="sxs-lookup"><span data-stu-id="82ad5-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="82ad5-109">Avage administraatoriõigustes Käsuviip, kliki - **Start**, paremklõpsake **käsku Käsuviip**ja seejärel klõpsake käsku **Käivita administraatorina**.</span><span class="sxs-lookup"><span data-stu-id="82ad5-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="82ad5-110">Tüüp *dsregcmd /leave* ja vajutage **Enter**.</span><span class="sxs-lookup"><span data-stu-id="82ad5-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="82ad5-111">Kui kõrvaklapid *dsregcmd /join* tüüp ja vajutage **Enter**.</span><span class="sxs-lookup"><span data-stu-id="82ad5-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="82ad5-112">Kui valmis, sulgege selle Käsuviip.</span><span class="sxs-lookup"><span data-stu-id="82ad5-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="82ad5-113">Taaskäivitage arvuti ja logige OneDrive'i.</span><span class="sxs-lookup"><span data-stu-id="82ad5-113">Reboot the computer, and log into OneDrive.</span></span>