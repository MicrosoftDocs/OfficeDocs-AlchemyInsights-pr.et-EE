---
title: Viga saatmisel e-post blokeeritud SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402255"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="98aa0-102">Viga saatmisel e-post: kliendi vastuvõtva blokeerida Spamhaus</span><span class="sxs-lookup"><span data-stu-id="98aa0-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="98aa0-103">Saadetud sõnumi IP-aadress on nende omanduses [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)plokk.</span><span class="sxs-lookup"><span data-stu-id="98aa0-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="98aa0-104">Blokeeritud Spamhaus võib olla ohustatud kontod ohus avalik IP-aadress ja Interneti-teenuse pakkuja (ISP) poliitika masinad.</span><span class="sxs-lookup"><span data-stu-id="98aa0-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="98aa0-105">Võimalikud parandused on:</span><span class="sxs-lookup"><span data-stu-id="98aa0-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="98aa0-106">Blokeeritud sissetulevad sõnumid Office 365 kui teil kontrollida allikas e-posti server, peate põhjuse ja eemaldada plokk Spamhaus veebilehel.</span><span class="sxs-lookup"><span data-stu-id="98aa0-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="98aa0-107">Blokeeritud sissetulevate teadete kui allika IP-aadress kuulub kellelegi teisele Office 365 aadressi omanik peab eemaldama ploki Spamhaus veebilehel.</span><span class="sxs-lookup"><span data-stu-id="98aa0-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="98aa0-108">Kui IP-aadress on poliitika Blokeeri nimekirja (PBL), omanik eri staatilist IP-aadressi määrata või eemaldada aadress on PBL.</span><span class="sxs-lookup"><span data-stu-id="98aa0-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="98aa0-109">Blokeeritud väljaminevad sõnumid teie Office 365 domeeni, saate selle tõrke, kui sõnumid on viidud läbi 3. osapoole teenust.</span><span class="sxs-lookup"><span data-stu-id="98aa0-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="98aa0-110">WHOIS lookup tööriist abil saate leida blokeeritud IP aadressi omanik.</span><span class="sxs-lookup"><span data-stu-id="98aa0-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

