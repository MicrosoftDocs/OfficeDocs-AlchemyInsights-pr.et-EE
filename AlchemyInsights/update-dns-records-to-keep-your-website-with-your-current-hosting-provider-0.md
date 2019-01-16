---
title: Värskendada DNS-kirjete hoida oma veebilehel koos oma praeguse hosting teenust
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28285428"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="61233-102">Värskendada DNS-kirjete hoida oma veebilehel koos oma praeguse hosting teenust</span><span class="sxs-lookup"><span data-stu-id="61233-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="61233-103">Leheküljel [Domeenid](https://portal.office.com/adminportal/home#/Domains) domeenide loendis Valige domeen, mida kasutate oma veebilehel, ja seejärel valige paan Dokumendihaldus **DNS-i sätted** .</span><span class="sxs-lookup"><span data-stu-id="61233-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="61233-104">Valige **+ uue kohandatud kirje** ja tippige järgmine:</span><span class="sxs-lookup"><span data-stu-id="61233-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="61233-105">Sisestage **DNS-i tüüp** : **(aadress)**</span><span class="sxs-lookup"><span data-stu-id="61233-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="61233-106">**Hosti nimi või pseudonüüm**, tippige järgmine:**@**</span><span class="sxs-lookup"><span data-stu-id="61233-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="61233-107">**IP-aadress**tippige veebisaidi, kus on praegu majutatud (näiteks 172.16.140.1) staatiline IP-aadress.</span><span class="sxs-lookup"><span data-stu-id="61233-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="61233-p101">See peab olema koduleht, mitte *dünaamilise* IP-aadressi *staatilise* IP-aadressi. Kohas, kus teie koduleheküljel on hostitud veendumaks, et avaliku veebisaidi staatilisi IP-aadressi saamiseks pöörduge.</span><span class="sxs-lookup"><span data-stu-id="61233-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="61233-110">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="61233-110">Select **Save**.</span></span> 
    
<span data-ttu-id="61233-111">Lisaks saate luua CNAME-kirje aitab kasutajatel leida oma veebilehel.</span><span class="sxs-lookup"><span data-stu-id="61233-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="61233-112">Valige **+ uue kohandatud kirje** ja tippige järgmine:</span><span class="sxs-lookup"><span data-stu-id="61233-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="61233-113">Sisestage **DNS-i tüüp** : **CNAME (pseudonüüm)**</span><span class="sxs-lookup"><span data-stu-id="61233-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="61233-114">**Hosti nimi või pseudonüüm**, tippige järgmine: **www**</span><span class="sxs-lookup"><span data-stu-id="61233-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="61233-115">**Punktid aadressile**, tippige domeeni nimi (FQDN) oma veebilehel (nt contoso.com).</span><span class="sxs-lookup"><span data-stu-id="61233-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="61233-116">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="61233-116">Select **Save**.</span></span> 
    

