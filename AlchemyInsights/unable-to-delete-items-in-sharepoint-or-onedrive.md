---
title: SharePointi või OneDrive ' is ei saa üksusi kustutada
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049513"
---
# <a name="unable-to-delete-items"></a>Üksusi ei saa kustutada

Kas SharePointi üksuste kustutamisel on probleeme?

- Veenduge alati, et teil on üksuse kustutamiseks [vajalikud õigused](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) või kui [saidikogumi administraator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) proovib üksust eemaldada.

- Veenduge, et üksusel pole [säilituspoliitika](https://docs.microsoft.com/office365/securitycompliance/retention-policies) seadistust.

- Veenduge, et üksus on [välja möllitud](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) teisele kasutajale.

- Lõpuks administraatorid saavad kasutada [SharePointi mustrid ja tavad](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), mis sisaldab teegi PowerShelli käske, mis võimaldavad teil sooritada keerukaid haldustoiminguid, näiteks jõu kustutamine kangekaelsed üksused.
- [Eemalda PNP-fail](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Eemalda PNP-kaust](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-loendi üksuse eemaldamine](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Eemalda PNP-loend](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Eemalda PNP-väli (veerg)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)