---
title: SharePoint Designeri ühenduse probleemid
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051709"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designeri ühenduse probleemid 

Kui SharePoint Designeri esineb SharePointi saitidele ühenduse probleemid, proovige järgmisi ühiseid lahendusi.

1. samm: Veenduge, et SharePoint Designer 2013 värskendatakse [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja [2 August 2016 värskendus SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2. samm: tühjendage kohaliku vahemälu failid:

1. Sulgege SharePoint Designer 2013.

2. Eemaldage kohalikus arvutis kõik failid, mis on leitud igas järgmises kaustas.

    - %AppData%\microsoft\veebiserveri Ekstensions\cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Avage SharePoint Designer 2013 ja sisestage konto uuesti, et näha, kas see töötab.

3. samm: [lubage kaasaegne autentimine Office 2013 Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Samm 4: Administraatorid peavad **lubama kohandatud skripti** SharePointi administreerimiskeskuse sätetes SharePoint Designeri ühenduse lubamiseks. Lisateavet leiate teemast [kohandatud skripti lubamine või vältimine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


