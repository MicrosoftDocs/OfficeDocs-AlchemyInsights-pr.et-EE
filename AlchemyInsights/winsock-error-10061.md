---
title: 1554 Winsock-tõrge 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e82e90b670235848105636fb2039ed60d3b93c67
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364909"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="d0e01-102">Winsocki tõrge 10061</span><span class="sxs-lookup"><span data-stu-id="d0e01-102">Winsock error 10061</span></span>

<span data-ttu-id="d0e01-103">See tähendab, et Office 365 ei saanud luua TCP pesa (ühendus) Sihthosti.</span><span class="sxs-lookup"><span data-stu-id="d0e01-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="d0e01-104">Selle tõrke põhjuseks enamasti oma tulemüüri konfiguratsiooni osas probleemi.</span><span class="sxs-lookup"><span data-stu-id="d0e01-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="d0e01-105">Probleemi lahendamiseks kontrollige neid sätteid:</span><span class="sxs-lookup"><span data-stu-id="d0e01-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="d0e01-106">Kontrollige oma tulemüüri konfiguratsiooni teabe [Office 365 URL-id](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) ja IP-aadressid</span><span class="sxs-lookup"><span data-stu-id="d0e01-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="d0e01-107">Kui viga ilmneb et Exchange Online kaitse (EOP), sa peaks on varem teatatud muudatusi [Exchange Online kaitse IP-aadressid](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="d0e01-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="d0e01-108">Veenduge, et teie Interneti-teenuse pakkuja (ISP) ei blokeeri sadama.</span><span class="sxs-lookup"><span data-stu-id="d0e01-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="d0e01-109">Nutika hosti ja sihtarvutite serveri sätteid oma pistikud kontrollida.</span><span class="sxs-lookup"><span data-stu-id="d0e01-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="d0e01-110">Pange tähele, et Office 365 ei blokeerida *sissetulevad* ühendused sel viisil.</span><span class="sxs-lookup"><span data-stu-id="d0e01-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
