---
title: Faili avamine kirjutuskaitstuna
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.openlocfilehash: 5c28d5f1c6951971aab329060e24b8458e848dd7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525667"
---
# <a name="file-open-read-only"></a><span data-ttu-id="39d06-102">Faili avamine kirjutuskaitstuna</span><span class="sxs-lookup"><span data-stu-id="39d06-102">File open read-only</span></span>

<span data-ttu-id="39d06-103">Võib juhtuda, et kui avate faile, nad avada kirjutuskaitstuna.</span><span class="sxs-lookup"><span data-stu-id="39d06-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="39d06-104">Mõnel juhul, see on turvalisuse lisamiseks nagu kui avate faile veebis ja muul ajal, see võib olla tingitud säte, mida saab muuta.</span><span class="sxs-lookup"><span data-stu-id="39d06-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="39d06-105">Siin on mõned sammud saab võtta, seda muuta ja mõnel juhul, kui fail avatakse kirjutuskaitstuna.</span><span class="sxs-lookup"><span data-stu-id="39d06-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="39d06-106">**Minu viirusetõrje põhjustab neid avada kirjutuskaitstud**</span><span class="sxs-lookup"><span data-stu-id="39d06-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="39d06-107">Mõned viirusetõrjeprogrammid võivad teid kaitsta potentsiaalselt ohtlike failide avamine need kirjutuskaitstud.</span><span class="sxs-lookup"><span data-stu-id="39d06-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="39d06-108">Peate oma viirusetõrje pakkuja õppida nende sätete kontrollimiseks.</span><span class="sxs-lookup"><span data-stu-id="39d06-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="39d06-109">BitDefender, näiteks, on sisu lisamise taotluse välistused siin: [Kuidas lisada taotluse või protsesside väljajätt Bitdefender juhtimiskeskus](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="39d06-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="39d06-110">**Failiatribuutide seatakse kirjutuskaitstud?**</span><span class="sxs-lookup"><span data-stu-id="39d06-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="39d06-111">Kontrollige faili atribuute, paremklõpsake failil ja käsku Atribuudid.</span><span class="sxs-lookup"><span data-stu-id="39d06-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="39d06-112">Kui kirjutuskaitstud atribuut on märgitud, saate Lülita see ja klõpsake nuppu OK.</span><span class="sxs-lookup"><span data-stu-id="39d06-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="39d06-113">**Sisu on kaitstud vaates**</span><span class="sxs-lookup"><span data-stu-id="39d06-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="39d06-114">Internetist ja teiste potentsiaalselt ebaturvalistest kohtadest saadud failid võivad sisaldada viirused, ussid ja muud tüüpi ründevara, mis võib teie arvutit kahjustada.</span><span class="sxs-lookup"><span data-stu-id="39d06-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="39d06-115">See on tavaliselt e-posti manuseid või allalaaditud failide puhul.</span><span class="sxs-lookup"><span data-stu-id="39d06-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="39d06-116">Teie arvuti kaitsmiseks on need potentsiaalselt ebaturvalistest kohtadest saadud failid kaitstud vaates avatud.</span><span class="sxs-lookup"><span data-stu-id="39d06-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="39d06-117">Kaitstud vaate kasutamisel saate faili lugeda ja riske vähendades selle sisu kuvamiseks.</span><span class="sxs-lookup"><span data-stu-id="39d06-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="39d06-118">Kaitstud vaate ja sätete muutmise kohta lisateabe saamiseks vaadake seda: [mis on kaitstud vaade?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="39d06-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="39d06-119">**OneDrive on täis?**</span><span class="sxs-lookup"><span data-stu-id="39d06-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="39d06-120">Kui fail on salvestatud OneDrive ja OneDrive salvestusruumi on täis, ei saa dokumenti salvestada, kuni olete alusel määratud ruumist.</span><span class="sxs-lookup"><span data-stu-id="39d06-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="39d06-121">Saate OneDrive'is Tasuta veebiruumi klõpsake teatamine center OneDrive'i ikooni ja käsku Halda salvestusruumi või võite minna [http://onedrive.live.com](http://onedrive.live.com), logige sisse ja märkida kasutatud ruumi alumises vasakul ekraani.</span><span class="sxs-lookup"><span data-stu-id="39d06-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="39d06-122">**Kas Office on aktiveeritud?**</span><span class="sxs-lookup"><span data-stu-id="39d06-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="39d06-123">Kui Office pole aktiveeritud või kui tellimus on aegunud, siis võiks ainult vähendatud funktsionaalsusega režiimis.</span><span class="sxs-lookup"><span data-stu-id="39d06-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="39d06-124">Kuidas aktiveerida Office'i Lisateavet: [litsentsimata toode ja aktiveerimistõrgete kontoris](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="39d06-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="39d06-125">**Kui kõik muu ebaõnnestub...**</span><span class="sxs-lookup"><span data-stu-id="39d06-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="39d06-126">Taaskäivitage arvuti</span><span class="sxs-lookup"><span data-stu-id="39d06-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="39d06-127">Office'i värskendusi installida</span><span class="sxs-lookup"><span data-stu-id="39d06-127">Install Office updates</span></span>
    
- <span data-ttu-id="39d06-128">Office Online remont</span><span class="sxs-lookup"><span data-stu-id="39d06-128">Perform an Online repair of Office</span></span>
    

