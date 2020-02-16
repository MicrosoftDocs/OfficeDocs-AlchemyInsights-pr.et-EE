---
title: Office ' i rakenduste kinnitamine teie konto on vigane oleku sõnum
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969385"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Office ' i rakenduste kinnitamine "teie konto on vigane olekus"

Selle tõrke lahendamiseks proovige mõjutatud arvutis järgmisi suvandeid.

- Avage Office ' i rakendus, valige **fail** > **konto** > **Logi välja kõik kontod**. Logige uuesti sisse, kasutades sobivat litsentsi kasutajakontot. Üksikasjaliku teabe saamiseks vaadake [Office ' i kontosid](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , kasutades Windowsi mandaat Manager.<br>
  **Märkus:** Office 2016 registri teed on muutunud 16,0. Näiteks \Software\Microsoft\Office\16.0\Common\Identity\
- Mõjutatud arvuti, seadke EnableADAL = 0, kasutades järgmisi samme:  
     1. Paremklõpsake Windowsi nuppu ja valige **Käivita**. Väljale **Ava** tippige **käsk regedit**ja seejärel valige **OK**.
     2. Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige **Jah** .
    3. Registriredaktori, lisage DWORD-väärtus EnableADAL sätte 0 all HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Kui tõrge ilmneb samal ajal Office 365, kasutades Office 2013, [lubage kaasaegne autentimine](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) Office ' i kliendi.

Lisateabe saamiseks vaadake, [Kuidas teha tõrkeotsingut mitte-brauseri rakendused, mis ei saa sisse logida Office 365, Azure või Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).
