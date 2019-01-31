---
title: Järelevalve juurdepääsu
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656563"
---
# <a name="monitoring-conditional-access"></a>Järelevalve juurdepääsu

Saavad juurdepääsu kasutajad saavad selle ettevõtte juurdepääsu nõuetele ei vasta. Probleemi lahendamiseks soovitame ühte või mitut järgmistest lahendustest:
  
- Kui seade on eeldada, et olla kaasatud, nõustada ettevõtte portaali rakendust ja veenduge, et see on ettevõtte portaali kasutaja. Kui seda pole, peaks kasutaja seadet registreerida.
    
- Minge Azure'i portaal **Intune \> seade vastavust**. **Kuvari** all klõpsake **seadme vastavust**. Saate vaadata oma seadme vastavuse aruandes veendumaks, et kasutaja seade on märgitud vastavuses. 
    
- Minge Azure'i portaal **Intune \> seade vastavust**. Klõpsake jaotises **Halda**ja **poliitika**. Täitmise poliitika loendis kontrollida, et profiil on oma kasutaja seadmele määratud. Kui ühtegi profiili on määratud, siis Intune ei saa kinnitada seadme vastavust oleku. 
    
- Muuta kasutaja juurdepääsu määramine.
    
1. Minge Azure'i portaal **Intune \> juurdepääsu \> poliitika**
    
2. Valige loendist reeglid
    
3. Klõpsake suvandit **kasutajad ja rühmad**
    
4. Keegi poliitika suunata need lisada **kaasamisloendis** . Tagamaks, et isik on välja jäetud poliitikast, lisada need **välistada** nimekirja. 
    
Loe edasi: [Monitor tingimusjuurdepääsuseadmete kuidas](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

