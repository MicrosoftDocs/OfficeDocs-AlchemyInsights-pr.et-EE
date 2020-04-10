---
title: Tingimusjuurdepääsu poliitikad
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 8ce41d007988f2a45f1ded385ae50ac3def97c1b
ms.sourcegitcommit: 9923ce61344e22c4490549b12f65fa2896490b1f
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/01/2020
ms.locfileid: "43100444"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="82e3f-102">Tingimusjuurdepääsu poliitikad</span><span class="sxs-lookup"><span data-stu-id="82e3f-102">Conditional Access policies</span></span>

<span data-ttu-id="82e3f-103">Tingimusjuurdepääs on Azure Active Directory funktsioon, mis võimaldab teil keskkonna rakendustele juurdepääsuks jõustada juhtelemente, mis põhinevad teatud tingimustel ja mida saab ühes kohas hallata.</span><span class="sxs-lookup"><span data-stu-id="82e3f-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="82e3f-104">Lisateavet leiate teemast [Azure Active Directory tingimusjuurdepääs](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="82e3f-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="82e3f-105">**Märkus**. Kui teie rentnik loodi pärast 21. oktoobrit 2019 ja teilt küsitakse ootamatult mitmikautentimist, olete tõenäoliselt oma rentnikus lubanud [turvalisuse vaikesätted](http://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="82e3f-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="82e3f-106">**Turvalisuse vaikesätete haldamine**</span><span class="sxs-lookup"><span data-stu-id="82e3f-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="82e3f-107">Logige oma üldadministraatori identimisteabega [halduskeskusse](https://go.microsoft.com/fwlink/p/?linkid=834822) sisse.</span><span class="sxs-lookup"><span data-stu-id="82e3f-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="82e3f-108">Avage [Azure Active Directory atribuudid](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="82e3f-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="82e3f-109">Lehe allosas klõpsake suvandit **Turvalisuse vaikesätete haldamine**.</span><span class="sxs-lookup"><span data-stu-id="82e3f-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="82e3f-110">Turvalisuse vaikesätete lubamiseks klõpsake valikut **Jah** või nende keelamiseks valikut **Ei**.</span><span class="sxs-lookup"><span data-stu-id="82e3f-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>