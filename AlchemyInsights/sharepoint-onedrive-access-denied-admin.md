---
title: Juurdepääs keelatud sõnumite tõrkeotsing
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751272"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Juurdepääs keelatud sõnumite tõrkeotsing SharePointi/OneDrive ' i administreerimiskeskuses

Kui teil on juurdepääs keelatud sõnumi sirvimisel SharePointi/OneDrive ' i administreerimiskeskus, veenduge, et [määrata litsentsi kasutajale](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Kui kasutajal on litsents, peaksite ka veenduma, et neile [määratakse administraatoriroll](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , mis pääseb juurde administreerimiskeskustele.

See probleem võib ilmneda ka siis, kui kasutaja on kustutatud ja uuesti loodud sama kasutaja turvasubjektinimi (UPN). Uus konto on loodud, kasutades erinevaid PUID (Passporti kordumatu ID) väärtus. Kui kasutaja proovib pääseda saidikogumi või oma OneDrive, kasutaja on vale PUID. Teine stsenaarium hõlmab kataloogi sünkroonimine Active Directory organisatsiooniüksusele (OU). Kui kasutajad on juba SharePointi sisse logitud ja seejärel teisaldatakse teise OU ja uuesti SharePoint, need võivad ilmneda probleem.

Selle probleemi lahendamiseks peaksite taastama algse UPN juhiseid artiklis, [taastada kasutaja Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Märkus: kui OneDrive või SharePointi administreerimiskeskus pole saadaval mitmele kasutajale, kellel oli varem juurdepääs, võib olla ajutine teenuse probleem.  [Kontrollige teenuse tervise armatuurlauda](https://portal.office.com/adminportal/home#/servicehealth).


