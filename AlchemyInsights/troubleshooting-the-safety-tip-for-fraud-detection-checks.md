---
title: Tõrkeotsingu ohutuse otsa pettuste avastamiseks kontrollib
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353245"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="2c876-102">Tõrkeotsingu ohutuse otsa pettuste avastamiseks kontrollib</span><span class="sxs-lookup"><span data-stu-id="2c876-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="2c876-103">Kui teil on saada ohutuse tip, mis ütleb "saatja ei meie pettuste avastamise kontrolli ja võib olla, kes need olevat" siis Saatja DKIM või SPF autentimise kontrolli läbida.</span><span class="sxs-lookup"><span data-stu-id="2c876-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="2c876-104">Parim viis probleemi lahendamiseks on saatja ise lubada.</span><span class="sxs-lookup"><span data-stu-id="2c876-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="2c876-105">Kui saatja saadab teie nimel, peate lubavad lisades saatja IP-aadress teie SPF-kirje.</span><span class="sxs-lookup"><span data-stu-id="2c876-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="2c876-106">Lisateavet vt [tõrkeotsing punane (kahtlane) ohutuse otsa pettuste avastamiseks kontrollib](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="2c876-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="2c876-107">Siin on mõned lingid, mis aitavad:</span><span class="sxs-lookup"><span data-stu-id="2c876-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="2c876-108">Kuidas Office 365 kasutab saatja poliitilise raamistiku (SPF), et vältida võltsimist</span><span class="sxs-lookup"><span data-stu-id="2c876-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="2c876-109">Seadistada SPF Office 365, mis aitab vältida võltsimist</span><span class="sxs-lookup"><span data-stu-id="2c876-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
