---
title: MDATP tõrkeotsing Mac-arvutis
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694282"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="a0762-102">MDATP tõrkeotsing Mac-arvutis</span><span class="sxs-lookup"><span data-stu-id="a0762-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="a0762-103">Kui käsitsi installimine nurjub, kuvatakse installiviisardi lehel **Kokkuvõte** järgmine tõrketeade:</span><span class="sxs-lookup"><span data-stu-id="a0762-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="a0762-104">"Installimisel ilmnes tõrge.</span><span class="sxs-lookup"><span data-stu-id="a0762-104">"An error occurred during installation.</span></span> <span data-ttu-id="a0762-105">Installeril ilmnes tõrge, mis põhjustas installi nurjumise.</span><span class="sxs-lookup"><span data-stu-id="a0762-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="a0762-106">Abi saamiseks pöörduge tarkvara tootja poole. "</span><span class="sxs-lookup"><span data-stu-id="a0762-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="a0762-107">MDM-i juurutuste korral kuvatakse lehel üldine installi tõrge.</span><span class="sxs-lookup"><span data-stu-id="a0762-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="a0762-108">Kuigi me ei kuva lõppkasutajatele täpseid vigu, hoiame logifaili installimisega **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="a0762-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="a0762-109">Iga installimise seanss lisatakse sellele logifaili.</span><span class="sxs-lookup"><span data-stu-id="a0762-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="a0762-110">Ainult viimase installimise seansi väljundiks kasutage `sed` .</span><span class="sxs-lookup"><span data-stu-id="a0762-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="a0762-111">Lisateavet leiate teemast [Microsoft DEFENDERI ATP for Maci installimisega seotud probleemide tõrkeotsing](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="a0762-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
