---
title: Säilituspoliitikate Exchange'i administraatori Center ei tööta
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 73e8db432afccb73b872ec7a3ce84c25f1ba7f25
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786766"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Säilituspoliitikate Exchange'i administraatori Center

 **Probleemi:** Vastloodud või Exchange'i administraatori Center uuendatud säilituspoliitikate ei taotle postkastidesse või üksusi ei arhiivi postkasti või kustutatakse. 
  
 **Root põhjused:**
  
- Põhjuseks võib olla peab **Hallatud kaustade abiline** on töödeldud postkasti. Hallatud kaustade abiline üritab teie pilvepõhise organisatsiooni iga seitsme päeva tagant iga postkasti töötlema. Kui muudate säilitussilti või rakendate postkastile muu säilituspoliitika, saate oodata, kuni õnnestus kausta aidata postkasti töötleb või käivitada cmdleti Start-ManagedFolderAssistant alustada abiline töötlemiseks konkreetne postkasti. Cmdlet-käsu käitamine on kasulik testimiseks või tõrkeotsinguks säilituspoliitika või säilitussildi sätete. Külastage lisateabe saamiseks [käivitada hallatud kaustade abiline](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Lahendus:** Alustada abiline konkreetsele postkastile järgmine käsk: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- See võib ilmneda ka siis, kui **RetentionHold** on **lubatud** postkasti. Kui postkast on saanud RetentionHold, säilituspoliitika postkastis ei töötle selle aja jooksul. Rohkem teavet vt RetentionHold sätte puhul: [Postkasti säilituse ooteloleku](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Lahendus:**
    
  - Kindla postkasti [EKSO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShelli RetentionHold sisselülitamiseks oleku kontrollimiseks:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Käivitage järgmine käsk **keelata** RetentionHold konkreetse postkasti: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Nüüd käivitage uuesti Managed kausta assistent:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Märkus:** Kui postkast on väiksem kui 10 MB, abiline ei töötleb automaatselt postkasti. 
  

