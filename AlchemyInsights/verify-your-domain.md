---
title: Kontrollige oma domeeni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 3dd96a9731cfd75882dd3bb397005b19d471c882
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531355"
---
# <a name="verify-your-domain"></a><span data-ttu-id="41c05-102">Kontrollige oma domeeni</span><span class="sxs-lookup"><span data-stu-id="41c05-102">Verify your domain</span></span>

 <span data-ttu-id="41c05-103">**Kirje pole ilmselt värskendada Interneti.**</span><span class="sxs-lookup"><span data-stu-id="41c05-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="41c05-104">Tavaliselt kulub vaid paar minutit meile vaadata uue kirje, kuid vahel võib võtta aega kuni paar tundi.</span><span class="sxs-lookup"><span data-stu-id="41c05-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="41c05-105">Kui see on juba ammu oodanud, kontrollige üle, et te olete kopeerimisel ja kleepimisel TXT Taatlusprotokolli täpne väärtus kell DNS host.</span><span class="sxs-lookup"><span data-stu-id="41c05-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="41c05-106">Üks levinud küsimus on ka selle "MS =" osa kirje.</span><span class="sxs-lookup"><span data-stu-id="41c05-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="41c05-107">Seda on vaja liiga!</span><span class="sxs-lookup"><span data-stu-id="41c05-107">We need that too!</span></span>

- <span data-ttu-id="41c05-108">Mõned DNS hosts, pead võtma lisatööd (DNS-kirje salvestamise) tsooni faili salvestamiseks nii, et see update Internetis.</span><span class="sxs-lookup"><span data-stu-id="41c05-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="41c05-109">Veenduge, et salvestate muudatused nii Office 365 näete ja kirje.</span><span class="sxs-lookup"><span data-stu-id="41c05-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
