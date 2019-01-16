---
title: Tõrkeotsingu kasutamine iOS seadmeid Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286152"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="a3f5d-102">Tõrkeotsingu kasutamine iOS seadmeid Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a3f5d-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="a3f5d-103">Läbi nende lahendamiseks nüüd allpool loetletud ressurssidele.</span><span class="sxs-lookup"><span data-stu-id="a3f5d-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="a3f5d-104">Mõned levinud tõrketeated ja lahendus:</span><span class="sxs-lookup"><span data-stu-id="a3f5d-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="a3f5d-p101">**Seadme Cap jõudis** Kasutajal on rohkem kui seadme seadmete. Läbi nende dokumentide [seade eemaldada](https://docs.microsoft.com/en-us/intune/devices-wipe) või [muuta seadme piirang](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="a3f5d-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="a3f5d-p102">**See teenus ei toeta. Puudub liitumise poliitika:** Apple Push teatamise teenus (APNid) määramine peab olema konfigureeritud või uuendada. Läbi [selle dokumendi](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) juhiseid, kuidas seda teha.</span><span class="sxs-lookup"><span data-stu-id="a3f5d-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="a3f5d-p103">**Kasutaja litsentsi tüüp sobimatu või Tundmatu kasutajanimi:** Kasutaja peab olema määratud Intune või EMS litsentsi. Läbi nende dokumentide kaudu litsentsi omistamiseks: [Office administreerimiskeskuse](https://docs.microsoft.com/en-us/intune/licenses-assign) või [Azure'i portaal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="a3f5d-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="a3f5d-111">Lisaressursse, mis probleemi lahendada:</span><span class="sxs-lookup"><span data-stu-id="a3f5d-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="a3f5d-p104">Diagnoosimiseks ja lahendamiseks ühise registreerimise rikete [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil. Läbi [selle dokumendi](https://docs.microsoft.com/en-us/intune/help-desk-operators) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="a3f5d-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="a3f5d-114">Läbi nende dokumentide nimekiri kõige sagedasemad vead, mis takistavad registreerimine ja lahendused igale: [tõrkeotsing juhend](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [tõrkeotsing doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="a3f5d-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="a3f5d-115">[Kuidas registreeruda Microsoft Intune iOS seadmeid](https://docs.microsoft.com/en-us/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="a3f5d-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span></span>
    

