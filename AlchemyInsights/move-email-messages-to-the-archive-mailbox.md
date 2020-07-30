---
title: Meilisõnumite ümberpaigutamine arhiivi postkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522767"
---
# <a name="move-email-to-the-archive-mailbox"></a>Meilisõnumite saatmine arhiivi postkasti

Kui soovite, et me käivitaks allpool nimetatud sätete automatiseeritud kontrollimised, valige nupp tagasi <--selle lehe ülaosas ja seejärel sisestage selle kasutaja meiliaadress, kellel on probleeme meilisõnumite teisaldamisega arhiivi postkasti.

1. Veenduge, et **arhiivi postkast** oleks lubatud. Kui seda ei ole, kasutage arhiivi postkasti lubamiseks [selles artiklis](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) toodud juhiseid.

2. Kui soovite arhiivi postkasti automaatselt arhiivida, **peab toimingu arhiivimiseks käsuga arhiivimine** olema seatud **automaatselt rakendama kogu postkasti (vaike) sildile**. Selle toimingu abil saate luua sildi: [arhiivi vaikevormingu](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Järgmisena lisage **arhiivi** silt oma säilituspoliitika. Valige Exchange ' i halduskeskus > **säilituspoliitika** , et lisada poliitikasse > **salvestatav nupp Salvesta** **arhiivi** .

4. Nüüd [Määra säilituspoliitika](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkreetse kasutaja postkasti. Sama poliitika rakendub nii **alg** -kui ka **arhiivi** postkastile.

Võimalik, et hallatava kausta assistent (MFA) peab käivitama ja rakendama kasutaja postkastile uusi sätteid. Kindla postkasti hallatava kausta abilise käivitamiseks käivitage järgmine käsk, [ühendades selle ekso PowerShelliga](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) .
  
Start-ManagedFolderAssistant – identiteet<name of the mailbox>

Lisateavet arhiivimise poliitika häälestamise kohta leiate teemast [postkastide arhiivimise ja kustutamise poliitika häälestamine](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  