---
title: Kustuta sõnum sündmused auditilogid tuvastada
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b358b7944b82182a8551d64701e6879a01816524
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539205"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Auditilogide kustutatud e-kirju

Alates jaanuarist 2019, Microsoft lülitab Postkasti auditilogi vaikimisi. Muul juhul vaadata Kustuta sõnum sündmused kindla kasutaja, peate käsitsi lubada auditeerimiseks toimingu delete. Kui postkasti auditi logimine on lubatud juba teie organisatsiooni jaoks või konkreetse kasutaja, tehke järgmist.

1. Logige sisse [Office 365 & vastavuse Turvakeskus](https://protection.office.com/)

2. Valige **Auditi logifaili Otsi**nuppu **Otsi ja uurimine** .

3. Valige kuupäevavahemik väljadele **Alguskuupäev** ja **lõppkuupäev** . Määrake kasutajanimi kasutaja, mida soovite uurida (kasutaja kustutatud üksused). Valige väljal **tegevuse** **kustutatud sõnumite kausta Kustutatud** ja **Moved sõnumite kausta Kustutatud**.

4. Klõpsake nuppu **Otsi**.

Tulemused, valige audit kirje. Hüpik üksikasjad nuppu **Lisateave**. Lisateavet kustutatud üksusi (nt teema ja kui see on kustutatud üksuse asukoht) kuvatakse väljal **AffectedItems** . **ClientInfoString** vara näitab kui kustutamise toimunud Outlooki, Outlook web (varasema nimega Outlook Web App) või teiste seadmetega.

Lisateabe saamiseks vt [Determining kes seadistada e-posti edasisuunamise postkasti](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Märkus**: te ei saa tuua auditi logifaili funktsiooniga kustutatud üksuste. Taastada kustutatud üksused Outlook veebis, Vaata [taastada kustutatud üksused Outlook Web Appis](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
