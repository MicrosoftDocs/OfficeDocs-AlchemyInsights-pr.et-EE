---
title: Tuvasta Kustuta sõnum sündmused auditilogi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716492"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Auditilogi kustutatud meilisõnumite jaoks

Alates jaanuarist 2019 Microsoft on sisse lülitada postkasti auditi logimise vaikimisi. Vastasel juhul saate mõne kindla kasutaja jaoks kustutada sõnumite kustutamise, peate käsitsi lubama kustutamise toimingute auditeerimine. Kui postkasti auditilogi on juba lubatud teie organisatsiooni või konkreetse kasutaja, järgige alltoodud juhiseid.

1. Logige sisse [Microsoft 365 Security & vastavuse keskus](https://protection.office.com/)

2. Klõpsake suvandit **Otsing ja uurimine** ning valige **auditilogi otsing**.

3. Saate **valida kuupäevavahemiku alguskuupäeva ja** **lõppkuupäeva** väljadel. Määrake kasutaja kasutajanimi, keda soovite uurida (kasutaja, kes kustutas üksused). Valige väljal **Tegevused** kustutatud **sõnumid kaustast** kustutatud ja **teisaldati sõnumid kustutatud üksuste kausta**.

4. Klõpsake suvandit **Otsing**.

Valige tulemustel auditikirje. Üksikasjade hüpik, klõpsake **rohkem teavet**. Välja **Affecteditems** kuvatakse Lisateave kustutatud üksuse kohta (nt teema rida ja üksuse asukoht, kui see kustutati). **Clientinfostring** atribuut kuvatakse, kui kustutamine ilmnes Outlookis, Outlook veebis (varem tuntud kui Outlook Web Appi) või mis tahes muu seade.

Lisateabe saamiseks vaadake määrates, [kes seadistada e-posti suunamine postkasti](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Märkus**: kustutatud üksusi ei saa tuua auditilogi funktsiooni abil. Kustutatud sõnumite allalaadimiseks Outlookis veebis vaadake teemat [Kustutatud üksuste taastamine rakenduses Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
