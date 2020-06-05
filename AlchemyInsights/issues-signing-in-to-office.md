---
title: Probleemid sisselogimisel Microsoft 365 rakendused
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579897"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="fcfdf-102">Tühi sisselogimiskuva rakenduses Microsoft 365 rakendused</span><span class="sxs-lookup"><span data-stu-id="fcfdf-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="fcfdf-103">Selle probleemi lahendamiseks proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="fcfdf-104">Installige uusimad värskendused [Windowsi](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office ' i](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)jaoks.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="fcfdf-105">Lähtesta Internet Exploreri suvandid: **tööriistadele**  >  **Interneti-suvandid**  >  **Täpsemad**  >  **Lähtesta Internet Exploreri sätted** (Pange tähele, et kaotate kohandatud sätted) ja seejärel proovige uuesti Office ' i sisse logida.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="fcfdf-106">Keelake Windows Defenderi Rakendusevalvur (WDAG) või muu sarnane tulemüür või viirusetõrje programm:</span><span class="sxs-lookup"><span data-stu-id="fcfdf-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="fcfdf-107">Juhtpaneel, avage **programmid**ja seejärel valige **Lülita Windowsi funktsioonid sisse või välja**.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="fcfdf-108">Kui Windows Defenderi Rakendusevalvur on lubatud, proovige seda keelata.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="fcfdf-109">**Märkus:** Võimalik, et peate arvuti taaskäivitama.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="fcfdf-110">Veenduge, et Microsoft. AAD. vahendajate plugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ei ole blokeeritud ühtegi rakendust või tulemüüri/viirusetõrje programm.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="fcfdf-111">[Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , kasutades Windowsi mandaat Manager.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="fcfdf-112">**Märkus:** Office 2016 registri teed on muutunud 16,0.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="fcfdf-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="fcfdf-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="fcfdf-114">Lisateabe saamiseks vaadake [ühenduse probleemid sisse logida pärast värskenduse Office 2016 ehitada 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="fcfdf-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>