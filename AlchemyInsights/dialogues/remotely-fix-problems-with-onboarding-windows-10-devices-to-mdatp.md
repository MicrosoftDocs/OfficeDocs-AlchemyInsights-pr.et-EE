---
title: Probleemide lahendamine Windows 10 seadmetes Microsoft Defenderi täiustatud ohtude kaitsega
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693007"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="e28e6-102">Probleemide lahendamine Windows 10 seadmetes Microsoft Defenderi täiustatud ohtude kaitsega</span><span class="sxs-lookup"><span data-stu-id="e28e6-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="e28e6-103">Kui teil on juurdepääs kaugarvutiga, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="e28e6-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="e28e6-104">Laadige alla [klientarvuti ühenduvuse analüsaatori](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostiline tööriist.</span><span class="sxs-lookup"><span data-stu-id="e28e6-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="e28e6-105">Ekstraktige ja käivitage MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="e28e6-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="e28e6-106">Otsige üles kaust MDATPClientAnalyzerResult, mis on sama kaust, kus analüsaatori tööriist alla laaditi.</span><span class="sxs-lookup"><span data-stu-id="e28e6-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="e28e6-107">Kui soovite otsida probleeme ühenduvuse või Interneti-puhverserveri sätetega, vaadake logifaili MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="e28e6-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="e28e6-108">Lisateavet leiate teemast [masinate pardal](https://go.microsoft.com/fwlink/?linkid=2143634)olevad probleemid.</span><span class="sxs-lookup"><span data-stu-id="e28e6-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
