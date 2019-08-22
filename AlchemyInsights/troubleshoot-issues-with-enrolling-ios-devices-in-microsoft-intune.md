---
title: Tõrkeotsingu kasutamine iOS seadmeid Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506921"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="5ca31-102">Tõrkeotsingu kasutamine iOS seadmeid Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5ca31-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="5ca31-103">Läbi nende lahendamiseks nüüd allpool loetletud ressurssidele.</span><span class="sxs-lookup"><span data-stu-id="5ca31-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="5ca31-104">Mõned levinud tõrketeated ja lahendus:</span><span class="sxs-lookup"><span data-stu-id="5ca31-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="5ca31-105">**Seadme Cap jõudis** Kasutajal on rohkem kui seadme seadmete.</span><span class="sxs-lookup"><span data-stu-id="5ca31-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="5ca31-106">Läbi nende dokumentide [seade eemaldada](https://docs.microsoft.com/intune/devices-wipe) või [muuta seadme piirang](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="5ca31-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="5ca31-107">**See teenus ei toeta. Puudub liitumise poliitika:** Apple Push teatamise teenus (APNid) määramine peab olema konfigureeritud või uuendada.</span><span class="sxs-lookup"><span data-stu-id="5ca31-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="5ca31-108">Läbi [selle dokumendi](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) juhiseid, kuidas seda teha.</span><span class="sxs-lookup"><span data-stu-id="5ca31-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="5ca31-109">**Kasutaja litsentsi tüüp sobimatu või Tundmatu kasutajanimi:** Kasutaja peab olema määratud Intune või EMS litsentsi.</span><span class="sxs-lookup"><span data-stu-id="5ca31-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="5ca31-110">Läbi nende dokumentide kaudu litsentsi omistamiseks: [Office administreerimiskeskuse](https://docs.microsoft.com/intune/licenses-assign) või [Azure'i portaal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="5ca31-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="5ca31-111">Lisaressursse, mis probleemi lahendada:</span><span class="sxs-lookup"><span data-stu-id="5ca31-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="5ca31-112">Diagnoosimiseks ja lahendamiseks ühise registreerimise rikete [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil.</span><span class="sxs-lookup"><span data-stu-id="5ca31-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="5ca31-113">Läbi [selle dokumendi](https://docs.microsoft.com/intune/help-desk-operators) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="5ca31-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="5ca31-114">Läbi nende dokumentide nimekiri kõige sagedasemad vead, mis takistavad registreerimine ja lahendused igale: [tõrkeotsing juhend](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ja [tõrkeotsing doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="5ca31-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="5ca31-115">[Kuidas registreeruda Microsoft Intune iOS seadmeid](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="5ca31-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

