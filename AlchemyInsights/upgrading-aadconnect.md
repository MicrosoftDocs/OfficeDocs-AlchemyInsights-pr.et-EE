---
title: 932 täiendamine AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 210f230929db72027a0f729b17901fe88eb45709
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757287"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="05381-102">Ühendage uuendada Azure AD</span><span class="sxs-lookup"><span data-stu-id="05381-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="05381-103">Vaikimisi on lubatud automaatne uuendus Azure AD ühenduse, mis võimaldab kiirendada teie arvutis Viimane versioon.</span><span class="sxs-lookup"><span data-stu-id="05381-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="05381-104">Kontrollige automaatse uuendamise sätteid, kasutada Azure AD PowerShelli cmdleti **Get-ADSyncAutoUpgrade** .</span><span class="sxs-lookup"><span data-stu-id="05381-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="05381-105">Cmdleti naaseb üks järgmistest väärtustest:</span><span class="sxs-lookup"><span data-stu-id="05381-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="05381-106">**Enabled**: automaatne uuendus on lubatud.</span><span class="sxs-lookup"><span data-stu-id="05381-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="05381-107">**Keelatud**: automaatne uuendus on keelatud.</span><span class="sxs-lookup"><span data-stu-id="05381-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="05381-108">**Suspended**: süsteem ei ole enam saada automaatsed versiooniuuendused.</span><span class="sxs-lookup"><span data-stu-id="05381-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="05381-109">Te ei saa konfigureerida see; See on süsteemi poolt seatud.</span><span class="sxs-lookup"><span data-stu-id="05381-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="05381-110">Lisateabe saamiseks vaadake [Automaatne uuendus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="05381-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="05381-111">Uusim versioon Azure AD ühenduse, minge [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="05381-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
