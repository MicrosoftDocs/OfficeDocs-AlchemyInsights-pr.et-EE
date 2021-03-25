---
title: Microsoft 365 rakenduste juurutamine rakenduses RDS, terminaliserveri või VDI ühiskasutusse antud rakenduse Enterprise jaoks
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200669"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="ceced-102">Microsoft 365 rakenduste juurutamine rakenduses RDS, terminaliserveri või VDI ühiskasutusse antud rakenduse Enterprise jaoks</span><span class="sxs-lookup"><span data-stu-id="ceced-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="ceced-103">Microsoft 365 rakenduste juurutamiseks kaugtöölaua teenuste (RDS), varem nimega terminaliteenuste abil, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="ceced-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="ceced-104">Teil peab olema Microsoft 365 äriplaani või Office 365 lepingu jaoks, mis sisaldab Microsoft 365 Enterprise ' i jaoks mõeldud rakendusi (nt Office 365 Enterprise E3 või Enterprise E5).</span><span class="sxs-lookup"><span data-stu-id="ceced-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="ceced-105">Microsoft 365 Apps for Business ja Microsoft 365 Business Standard lepingud ei sisalda Microsoft 365 Apps for Enterprise.</span><span class="sxs-lookup"><span data-stu-id="ceced-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="ceced-106">Peate lubama [ühiskasutatava arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="ceced-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="ceced-107">Samuti saate alla laadida ja käivitada [Microsofti tugiteenuste ja taastekonsooli abilise](https://aka.ms/SaRA_OfficeSCA_M365Portal) , et installida Office ' i ühiskasutusega arvuti aktiveerimise režiimis Microsoft 365 rakendused.</span><span class="sxs-lookup"><span data-stu-id="ceced-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="ceced-108">Lisateavet Office ' i juurutamise tööriista kasutamise eeltingimuste, häälestamise juhiste ja kohandatud installide kohta leiate teemast [microsofti 365 rakenduste juurutamine kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="ceced-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="ceced-109">Ühiskasutusega arvuti aktiveerimisega seotud tõrgete lahendamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="ceced-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="ceced-110">Lugege teemat [Office ' i jaoks mõeldud Microsoft 365 rakenduste ühiskasutusega arvuti aktiveerimisega seotud probleemide tõrkeotsing](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="ceced-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="ceced-111">Lugege artiklit [Microsoft 365 suurettevõtterakenduste aktiveerimisoleku lähtestamine](https://go.microsoft.com/fwlink/?linkid=2109218) (inglise keeles).</span><span class="sxs-lookup"><span data-stu-id="ceced-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="ceced-112">Kui soovite installida Microsoft 365 rakendusi RDS-ile Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätteid***, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="ceced-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="ceced-113">Vaadake, milline tellimus teil on.</span><span class="sxs-lookup"><span data-stu-id="ceced-113">Check what subscription you have.</span></span> <span data-ttu-id="ceced-114">[Vaadake, kuidas](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="ceced-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="ceced-115">Vajadusel aktiveerige mõni muu pakett.</span><span class="sxs-lookup"><span data-stu-id="ceced-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="ceced-116">[Vaadake, kuidas](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="ceced-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="ceced-117">Kui Office on juba RDS-serverisse installitud mis tahes muu Microsofti tellimuse kaudu, desinstallige see.</span><span class="sxs-lookup"><span data-stu-id="ceced-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="ceced-118">Näiteks **juhtpaneeli** käsuga  >  **Desinstalli programm**.</span><span class="sxs-lookup"><span data-stu-id="ceced-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="ceced-119">Kui teil on probleeme, desinstallige [Microsoft support ja Recovery Assistanti](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.</span><span class="sxs-lookup"><span data-stu-id="ceced-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="ceced-120">Rakenduses RDS logige sisse oma administraatori kontoga Microsoft 365 halduskeskus ja [installige Enterprise ' i jaoks microsoft 365](https://portal.office.com/OLS/MySoftware.aspx)' i rakendused.</span><span class="sxs-lookup"><span data-stu-id="ceced-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="ceced-121">Kui Office on installitud, ***Ärge avage ega logige sisse*** ühtegi Office ' i rakendusse.</span><span class="sxs-lookup"><span data-stu-id="ceced-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="ceced-122">RDS-serveris lubage ühiskasutusega arvuti aktiveerimine, redigeerides registrit, järgides järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="ceced-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="ceced-123">Paremklõpsake Kuva vasakus allnurgas nuppu Windows ja valige **Käivita**.</span><span class="sxs-lookup"><span data-stu-id="ceced-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="ceced-124">Tippige väljale Ava **käsk regedit** ja seejärel klõpsake **nuppu OK**.</span><span class="sxs-lookup"><span data-stu-id="ceced-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="ceced-125">Kui teilt küsitakse, kas soovite, et registriredaktori saaks teie seadmes muudatusi teha, valige **Jah** .</span><span class="sxs-lookup"><span data-stu-id="ceced-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="ceced-126">Lisage registriredaktori **SharedComputerLicensing** stringi väärtus, mille sätteks on HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="ceced-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="ceced-127">RDS-serveris ***logige sisse lõppkasutajana*** ja veenduge, [et ühiskasutusega arvuti aktiveerimine oleks lubatud Microsoft 365 rakenduste jaoks Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)' i jaoks.</span><span class="sxs-lookup"><span data-stu-id="ceced-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
