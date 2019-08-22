---
title: Rühma lisamine SharePointi saidil
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507843"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Probleemid, kui luua või rühma ühendatud saitidel SharePoint Online

On ühiseid teemasid kui ühendatud loomine või uuesti luua rühma saidi paar.

 Kui rühma ja sellega seotud saidi kustutanud ja soovite luua teisele saidile sama URL-iga, peate eelmisest jäädavalt eemaldada.

Lae [SPO halduskestas](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Rohkem infot kuidas alustada PowerShelli abil, vaadake [SharePoint Online halduskesta alustamine](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Eemalda saidi kustutada saidid kasutades [Eemalda-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShelli cmdlet-i.

Kui rühma ühendatud saidi loomisel kuvatakse hoiatus, teine rühm sama pseudonüüm on juba olemas, kontrollige [Office 365 halduskeskuse kaudu](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)olemasolevatesse gruppidesse. Probleemi lahendamiseks, olemasoleva rühma kustutada, kui see ei ole enam vajalik või luua saidi eri alias määratud.

On erinevaid viise, kuidas luua ja kasutada kaasaegseid sõprade SharePointiga.

Interneti Office 365 rühma olemasolevatel saitidel. Lisateavet leiate teemast [ühendamine Office 365 rühma, kasutades SharePointi kasutaja ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Office 365 rühma ühendatud saidi loomiseks peate luua meeskonnatöö veebisaidi. Lisateavet leiate teemast [loomine SharePointi meeskonnasaidi](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

