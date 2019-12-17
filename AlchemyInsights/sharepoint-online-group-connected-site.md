---
title: Rühma lisamine SharePointi saidile
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051097"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="4dc6a-102">Probleemid loomisel või rühma ühendatud saidid SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="4dc6a-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="4dc6a-103">Rühma ühendatud saidi loomisel või uuesti loomisel ilmnesid mõned tavalised probleemid.</span><span class="sxs-lookup"><span data-stu-id="4dc6a-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="4dc6a-104">Kui olete kustutanud rühma ja selle ühendatud saidi ning soovite luua sama URL-iga mõne muu saidi, peate eelmise saidi jäädavalt eemaldama.</span><span class="sxs-lookup"><span data-stu-id="4dc6a-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="4dc6a-105">Lae alla [SPO Management shelli](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="4dc6a-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="4dc6a-106">Lisateavet PowerShelli kohta alustamine, vaadake alustamine [SharePoint Online Management shelli](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="4dc6a-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="4dc6a-107">Eemaldage saidi kustutatud saidid kasutades [Eemalda SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShelli cmdlet-käsu.</span><span class="sxs-lookup"><span data-stu-id="4dc6a-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="4dc6a-108">Kui loote rühma ühendatud saidi ja kuvatakse hoiatus teine sama pseudonüümiga rühm on juba olemas, kontrollige olemasolevaid rühmi [Office 365 alates administreerimiskeskusest](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="4dc6a-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="4dc6a-109">Probleemi lahendamiseks kustutage olemasolev rühm, kui see ei ole enam vajalik või luua saidi teise alias määratud.</span><span class="sxs-lookup"><span data-stu-id="4dc6a-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="4dc6a-110">On erinevaid viise, kuidas luua ja kasutada tänapäevaseid rühmi SharePointiga.</span><span class="sxs-lookup"><span data-stu-id="4dc6a-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="4dc6a-111">Saate ühendada olemasolevad saidid Office 365 rühma.</span><span class="sxs-lookup"><span data-stu-id="4dc6a-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="4dc6a-112">Lisateabe saamiseks vaadake [Connect Office 365 rühma SharePointi kasutaja ineterface abil](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="4dc6a-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="4dc6a-113">Office 365 rühma ühendatud saidi loomiseks peate looma meeskonnatöö saidi.</span><span class="sxs-lookup"><span data-stu-id="4dc6a-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="4dc6a-114">Lisateavet leiate teemast [meeskonnatöö saidi loomine SharePointis](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="4dc6a-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

