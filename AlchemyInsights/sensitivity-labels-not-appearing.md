---
title: Tundlikkussilte ei kuvata
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 1326eca02044014a8e9c072fcc3e4cd3a41c7a9f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511648"
---
# <a name="sensitivity-labels-not-appearing"></a>Tundlikkussilte ei kuvata

Tundlikkuse sildid võimaldavad teil oma tundliku sisuga sisu klassifitseerida ja kaitsta. Neid saab luua Microsoft 365 vastavuse keskus, Microsoft 365 Turvakeskus või Microsoft 365 Security & vastavuse Center jaotises klassifikatsioon > tundlikkuse sildid. Selle funktsiooni kohta lisateabe saamiseks vaadake [tundlikkuse siltide ülevaade](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Kui konfigureerisite tundlikkuse silte, kuid neid ei kuvata Office ' i rakendustes, kontrollige järgmist.

- Kinnitage, et tundlikkuse silt on [avaldatud](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) soovitud kasutajatele ja rühmadele.

- Kinnitage, et kasutaja kasutab tundlikkussilte toetavat rakendust – vt [dokumendi tundlikkuse silte](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Kui [migreerite Azure ' i teabekaitse silte](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), arvestage [siin](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)loetletud kaalutlustega.

- Andmete kadu vältimine (DLP) tugi: praegu ainult Säilitussildid saab kasutada tingimus DLP poliitika.  Tundlikkuse sildid DLP poliitika tugi ei ole veel saadaval, kuid me töötame selle kallal.

- Kui tundlikkuse sildil on krüptimine lubatud, saate valida kas:
    - Määra õigused kohe
    - Luba kasutajatel õigusi määrata


Võimalike probleemide kohta lisateabe saamiseks vaadake [teadaolevad probleemid tundlikkuse sildid](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).