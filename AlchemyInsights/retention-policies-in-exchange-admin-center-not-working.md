---
title: Säilituspoliitikate Exchange'i administraatori Center ei tööta
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371294"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="12b09-102">Säilituspoliitikate Exchange'i administraatori Center</span><span class="sxs-lookup"><span data-stu-id="12b09-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="12b09-103">**Probleemi:** Vastloodud või Exchange'i administraatori Center uuendatud säilituspoliitikate ei taotle postkastidesse või üksusi ei arhiivi postkasti või kustutatakse.</span><span class="sxs-lookup"><span data-stu-id="12b09-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="12b09-104">**Root põhjused:**</span><span class="sxs-lookup"><span data-stu-id="12b09-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="12b09-105">Põhjuseks võib olla peab **Hallatud kaustade abiline** on töödeldud postkasti.</span><span class="sxs-lookup"><span data-stu-id="12b09-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="12b09-106">Hallatud kaustade abiline üritab teie pilvepõhise organisatsiooni iga seitsme päeva tagant iga postkasti töötlema.</span><span class="sxs-lookup"><span data-stu-id="12b09-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="12b09-107">Kui muudate säilitussilti või rakendate postkastile muu säilituspoliitika, saate oodata, kuni õnnestus kausta aidata postkasti töötleb või käivitada cmdleti Start-ManagedFolderAssistant alustada abiline töötlemiseks konkreetne postkasti.</span><span class="sxs-lookup"><span data-stu-id="12b09-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="12b09-108">Cmdlet-käsu käitamine on kasulik testimiseks või tõrkeotsinguks säilituspoliitika või säilitussildi sätete.</span><span class="sxs-lookup"><span data-stu-id="12b09-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="12b09-109">Külastage lisateabe saamiseks [käivitada hallatud kaustade abiline](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="12b09-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="12b09-110">**Lahendus:** Alustada abiline konkreetsele postkastile järgmine käsk:</span><span class="sxs-lookup"><span data-stu-id="12b09-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="12b09-111">See võib ilmneda ka siis, kui **RetentionHold** on **lubatud** postkasti.</span><span class="sxs-lookup"><span data-stu-id="12b09-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="12b09-112">Kui postkast on saanud RetentionHold, säilituspoliitika postkastis ei töötle selle aja jooksul.</span><span class="sxs-lookup"><span data-stu-id="12b09-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="12b09-113">Rohkem teavet vt RetentionHold sätte puhul: [Postkasti säilituse ooteloleku](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="12b09-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="12b09-114">**Lahendus:**</span><span class="sxs-lookup"><span data-stu-id="12b09-114">**Solution:**</span></span>
    
  - <span data-ttu-id="12b09-115">Kindla postkasti [EKSO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShelli RetentionHold sisselülitamiseks oleku kontrollimiseks:</span><span class="sxs-lookup"><span data-stu-id="12b09-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="12b09-116">Käivitage järgmine käsk **keelata** RetentionHold konkreetse postkasti:</span><span class="sxs-lookup"><span data-stu-id="12b09-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="12b09-117">Nüüd käivitage uuesti Managed kausta assistent:</span><span class="sxs-lookup"><span data-stu-id="12b09-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="12b09-118">**Märkus:** Kui postkast on väiksem kui 10 MB, abiline ei töötleb automaatselt postkasti.</span><span class="sxs-lookup"><span data-stu-id="12b09-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

