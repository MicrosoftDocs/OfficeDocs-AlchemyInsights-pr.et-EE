---
title: 1336 RecoverableItems kaust on täis
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28285413"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="6df04-102">Kausta Taastatavad üksused on täis</span><span class="sxs-lookup"><span data-stu-id="6df04-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="6df04-p101">Office 365 Exchange Online'i postkasti kausta Taastatavad üksused vaikimisi mahupiirang on 30 GB. Kausta Taastatavad üksused mahupiirang on automaatselt suurendada 100 GB kui postkasti otsuse ootele, eDiscovery ootele, pannakse või osale Office 365 säilituspoliitika.</span><span class="sxs-lookup"><span data-stu-id="6df04-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="6df04-105">Kui kausta Taastatavad üksused jõuab salvestuslimiidi, mõjutatakse postkasti funktsionaalsust järgmiselt:</span><span class="sxs-lookup"><span data-stu-id="6df04-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="6df04-106">Kasutaja ei saa kustutada postkastist üksusi.</span><span class="sxs-lookup"><span data-stu-id="6df04-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="6df04-107">Hallatud kaustade abiline ei saa kustutada kaupu säilitussildi või hallatavasse kausta seaded.</span><span class="sxs-lookup"><span data-stu-id="6df04-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="6df04-108">Postkastid, millel on lubatud ühe üksuse taastamine või ootele panna, ei saa kopeerimise kohta kirjutage lehe kaitse protsessi säilitada kasutaja muutis üksuste versioone.</span><span class="sxs-lookup"><span data-stu-id="6df04-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="6df04-109">Postkastide on postkasti kontroll-logi sisse lülitatud, salvestatakse postkasti auditi logi kannete auditite alamkausta kaustas Taastatavad üksused.</span><span class="sxs-lookup"><span data-stu-id="6df04-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="6df04-p102">Postkastide, mis ei ole registreeritud, saate kasutada administraatoritel on `Search-Mailbox -SearchDumpsterOnly -DeleteContent` käsu Exchange Online PowerShelli kustutada kausta Taastatavad üksused. Lisateabe saamiseks vaadake järgmisi teemasid:</span><span class="sxs-lookup"><span data-stu-id="6df04-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="6df04-112">Otsida ja kustutada sõnumeid</span><span class="sxs-lookup"><span data-stu-id="6df04-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="6df04-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="6df04-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="6df04-p103">Hoida postkastide administraatoritel on hold eemaldada, enne kui nad kustutatud üksuste kaustast Taastatavad üksused. Rohkem Lisateavet [taastatavate üksuste kausta kohta postkastidel hoidke üksuste kustutamine](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="6df04-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="6df04-p104">Aidata vältida liigset täielik kausta Taastatavad üksused, Administraatorid võivad suurendada taastatavate üksuste kaust postkastide hoida ja luua postkasti säilituspoliitika, mis teisaldab üksused kaustast Taastatavad üksused kasutaja arhiivi salvestuslimiidi postkasti. Vaata [Taastatavad üksused kvoot postkastide hoidke suurendada](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="6df04-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

