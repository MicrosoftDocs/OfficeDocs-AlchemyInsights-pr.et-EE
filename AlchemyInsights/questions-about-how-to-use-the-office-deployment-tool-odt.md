---
title: Küsimused Office ' i juurutamise tööriista (ODT) kasutamise kohta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698054"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Küsimused Office ' i juurutamise tööriista (ODT) kasutamise kohta

Office ' i juurutamise tööriista alla laadida [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Pärast faili allalaadimist käivitage iseavanev täitmisfail, mis sisaldab Office ' i Juurutustööriista täitmisfaili (setup. exe) ja näidiskonfiguratsioonifaili (Configuration. XML).
  
 **Välistada või eemaldada Microsoft 365 apps ettevõtte toodete klientarvutid:**
  
Kui installite Microsoft 365 apps Enterprise, saate välistada teatud tooted. Selleks järgige Office ' i ODT-ga installimiseks juhiseid, kuid lisage konfiguratsioonifailis Excludeappi element. Näiteks see konfiguratsioonifail installib kõik Microsoft 365 apps ettevõtte toodete peale Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office ' i juurutamise tööriista ülevaade](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

