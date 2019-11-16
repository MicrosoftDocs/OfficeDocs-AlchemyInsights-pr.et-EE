---
title: Probleemi tõrkeotsing-kasutajat ei leitud kataloogist
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768797"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ea889-102">Probleemi tõrkeotsing-kasutajat ei leitud kataloogist</span><span class="sxs-lookup"><span data-stu-id="ea889-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ea889-103">Kui kasutajad saavad tõrketeate "kasutajat ei leita" kataloogis, proovige uuesti, kui probleemi tüüp on kasutaja ei ole kataloog.</span><span class="sxs-lookup"><span data-stu-id="ea889-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ea889-104">Järgmised sammud saab lõpule viia probleemi tõrkeotsingu sooritamiseks.</span><span class="sxs-lookup"><span data-stu-id="ea889-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ea889-105">Veenduge, et e-posti kutse aktsepteeritud konto on sama konto, mida kasutatakse hiljem sisse logida.</span><span class="sxs-lookup"><span data-stu-id="ea889-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ea889-106">Veenduge, et kasutaja kasutab sama kontot kutse vastuvõtmiseks ja saidile sisselogimiseks.</span><span class="sxs-lookup"><span data-stu-id="ea889-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ea889-107">Lisateabe saamiseks vaadake, [Kuidas hallata pseudonüümid oma Microsofti konto</a> hallata Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="ea889-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ea889-108">Sirvige iga saidi (s), kus kasutaja saab tõrke.</span><span class="sxs-lookup"><span data-stu-id="ea889-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ea889-109">Lisage "/_layouts/15/People.aspx/membershipgroupid = 0" (sees kahekordsete jutumärkidega) saidi URL-i lõppu.</span><span class="sxs-lookup"><span data-stu-id="ea889-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ea889-110">Näide: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="ea889-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ea889-111">Valige loendist kasutaja.</span><span class="sxs-lookup"><span data-stu-id="ea889-111">Select the user from the list.</span></span>

- <span data-ttu-id="ea889-112">Klõpsake lindilt **kasutaja õiguste eemaldamine** .</span><span class="sxs-lookup"><span data-stu-id="ea889-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ea889-113">Lisa kasutaja tagasi ja saatke kutse kasutajale.</span><span class="sxs-lookup"><span data-stu-id="ea889-113">Add back the User and Resend the invite to the user.</span></span>

