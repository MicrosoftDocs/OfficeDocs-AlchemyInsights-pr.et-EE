---
title: EndPoint Manager – turbe etalonid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440880"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – turbe etalonid

Turbe etalonid on Windowsi sätete eelkonfigureeritud rühmad, mis aitavad teil neid asjaomaste turvalisuse töörühmade soovitatavaid turvalisuse seadistusi rakendada. Neid etalone saab kohandada, et pakkuda ainult soovitud seadistusi ja väärtusi. Lisateavet turbe etalonide kohta vaadake teemast [Intune’is Windows 10 seadmete konfigureerimiseks turbe etalonide kasutamine](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Nende toodete praegused etalonid on järgmised.

- Windows MDM-i turbesätted
- Microsoft Defender for Endpointi turve
- Microsoft Edge

Kõiki etalone värskendatakse perioodiliselt ja antakse välja astmeliste versioonidena. Iga versioon lisab ja/või eemaldab eelmise versiooni sätted, et tagada, et etalon vastaks praegustele juhistele. Lõpp-punkti turvalisuse turbe etalonide konsool võimaldab võrrelda erinevaid versioone, muutes versioonide vahelised muudatused nähtavaks.

Juhisteks selle kohta, kuidas saab kõige tõhusamalt muuta seda, milline lähtealuse versioon juurutatakse, vaadake teemast [Turbe etaloni profiilide haldamine Microsoft Intune’is](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Turbe etaloni juurutamise järel saate jälgida juurutamise olekut ja vaadata üle seadmepõhiselt seadistused.

**Märkus.** Etalonide aruandluse andmete ilmumiseks võib kuluda kuni 24 tundi alates algsest seadmes juurutamisest ja kuni 6 tundi edasiste värskenduste korral. 

Etaloni seadistuse mitte rakendumise kõige levinum põhjus on, kui erinev profiil kasutab sama seadistust. Seda stsenaariumit saab konkreetse seadme jaoks uurida, valides selle seadme turbe etaloni profiili sõlmest Seadme olek. Üksikasju vaadake teemast [Turbe etalonide konfliktide lahendamine](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).