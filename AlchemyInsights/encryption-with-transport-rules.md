---
title: Krüptimine transpordireeglitega
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813864"
---
# <a name="encryption-with-transport-rules"></a>Krüptimine transpordireeglitega

[Exchange’i halduskeskuses](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) saate meilivoo reeglites kasutada meilisõnumite krüptimise käivitamiseks Office’i sõnumikrüptimine (OME) funktsioone. Valige transpordireegli tingimuses suvand **Rakenda Office 365 sõnumikrüptimine ja õiguste kaitse**.

- Lisateavet vaadake teemast [Meilivoo reegli krüptimiseks määratlemine](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Kasutage PowerShellis cmlet-käsku [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) ja määrake parameeter *ApplyOME* väärtusele $true.
