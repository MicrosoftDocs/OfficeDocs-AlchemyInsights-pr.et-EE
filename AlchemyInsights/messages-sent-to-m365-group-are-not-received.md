---
title: Kõik rühma liikmed ei saa Microsoft 365 rühma saadetud sõnumeid kätte
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480679"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Kõik rühma liikmed ei saa Microsoft 365 rühma saadetud sõnumeid kätte

Veenduge, et kõik rühma liikmed oleksid meilisõnumite vastuvõtmise tellinud. Lugege artiklit [Rühma jälgimine Outlookis](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Kui soovite vaadata rühmameilisõnumid tellinud liikmete sõnumite olekut, käivitage [EXO PowerShellis](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true) järgmine käsk:

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Kasutage järgmist EXO PowerShelli käsku, et konfigureerida kõigi rühmaliikmete jaoks Microsoft 365 rühmale saadetud meilisõnumite vastuvõtmine oma postkastis:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Näide.

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`