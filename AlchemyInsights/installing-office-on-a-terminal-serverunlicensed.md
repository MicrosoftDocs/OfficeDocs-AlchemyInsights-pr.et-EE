---
title: Office ' i installimine terminaliserverisse-litsentsimata
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735385"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="4f430-102">Office ' i installimine terminaliserverisse</span><span class="sxs-lookup"><span data-stu-id="4f430-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="4f430-103">Office 365 ProPlusi juurutamine Windows Serveri abil kaugtöölaua teenuste (RDS), varem nimega Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="4f430-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="4f430-104">Peab teil olema Office 365 kava, mis sisaldab Office 365 ProPlus, näiteks Office 365 Enterprise E3 või Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="4f430-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="4f430-105">Office 365 Business ja Office 365 Business Premiumi plaanid ei sisalda Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="4f430-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="4f430-106">Peate lubama [ühiskasutusega arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="4f430-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="4f430-107">Kui soovite installida Office 365 ProPlus RDS Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätted***, toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="4f430-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="4f430-108">Kontrollige, milline Office 365 plaan teil on.</span><span class="sxs-lookup"><span data-stu-id="4f430-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="4f430-109">Vaadake, kuidas</span><span class="sxs-lookup"><span data-stu-id="4f430-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="4f430-110">Vajadusel aktiveerige mõni muu Office 365 plaan.</span><span class="sxs-lookup"><span data-stu-id="4f430-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="4f430-111">Vaadake, kuidas</span><span class="sxs-lookup"><span data-stu-id="4f430-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="4f430-112">Kui Office on juba installitud RDS server, kasutades muid Office 365 plaanid, desinstallige see.</span><span class="sxs-lookup"><span data-stu-id="4f430-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="4f430-113">Näiteks, minnes juhtpaneeli \> desinstallida programmi.</span><span class="sxs-lookup"><span data-stu-id="4f430-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="4f430-114">Kui teil on probleeme, desinstallige [Microsofti toe-ja Taasteabimehe](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.</span><span class="sxs-lookup"><span data-stu-id="4f430-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="4f430-115">RDS server, logige sisse Microsoft 365 halduskeskus administraatori kontoga ja [installige Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="4f430-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="4f430-116">Pärast Office ' i installimist ***Ärge avage ega logige sisse*** ühelegi Office ' i rakendustele.</span><span class="sxs-lookup"><span data-stu-id="4f430-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="4f430-117">RDS server, lubage ühiskasutusse antud arvuti aktiveerimine registri redigeerimisel toimige järgmiselt:</span><span class="sxs-lookup"><span data-stu-id="4f430-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="4f430-118">Paremklõpsake ekraani alumises vasakus nurgas asuvat Windowsi nuppu ja valige käsk Käivita.</span><span class="sxs-lookup"><span data-stu-id="4f430-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="4f430-119">Väljale Ava tippige **käsk regedit**ja seejärel valige OK.</span><span class="sxs-lookup"><span data-stu-id="4f430-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="4f430-120">Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige Jah.</span><span class="sxs-lookup"><span data-stu-id="4f430-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="4f430-121">Registriredaktoris lisada stringi väärtus **Sharedcomputerlicensing** sätte 1 all HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="4f430-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="4f430-122">RDS server, logige sisse ***lõppkasutaja*** ja [veenduge, et ühiskasutuses arvuti aktiveerimine on lubatud Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="4f430-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="4f430-123">Eeltingimused, setup juhiseid ja juhiseid kohandatud installi Office ' i juurutamise tööriista abil kohta lisateabe saamiseks vaadake [juurutamine office 365 ProPlus kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="4f430-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="4f430-124">Ühiskasutusega arvuti aktiveerimisega seotud tõrgete lahendamiseks vaadake teemat probleemide [tõrkeotsing ühiskasutusse antud arvuti aktiveerimisega Office 365 ProPlusi jaoks](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="4f430-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  