---
title: DLP reegel USA / UK passi Number ei tööta
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912092"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP - probleemid U.S. / UK passi numbrid

On teil probleeme **Andmete kaotsimineku vältimise (DLP)** ei tööta sisu sisaldava puhul on **U.S. / UK passi Number** kasutades DLP tundliku teabe tüüp O365? Sellisel juhul veenduge, et sisu sisaldab vajalikku teavet kui hinnatakse seda, mida otsib DLP poliitika. 
  
Näiteks on **U.S. / UK passi Number** konfigureeritud 75% usaldusnivoo, järgmine hinnatakse ja reegli käivitamiseks tuleb kindlaks 
  
- **[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Üheksa numbrit 
    
- **[Puhul:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Üheksa järjestikust numbrit 
    
- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole kontrollsumma 
    
- **[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP poliitika on 75% kindel, et ta ei avastanud seda tüüpi tundlikku teavet kui raadiuses 300 tähemärki: 
    
  - Funktsiooni Func_usa_uk_passport leiab sisu, mis ühtiks.
    
  - Märksõna: Keyword_passport ei leitud.
    
    Näiteks peale tingiksid jaoks on **U.S. / UK passinumber** poliitika: USA passi number 123456789 
    
Rohkem infot mis tuleb USA / UK passi Number tuvastada sisu, vt käesoleva artikli järgmist osa: [mida the tundliku teabe tüübid vaadata USA / UK passi Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Kasutades erinevaid sisseehitatud tundliku teabe tüüp, lugege järgmist teabe kohta, mida nõutakse muude: [mida the tundlik tüüpi teavet otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

