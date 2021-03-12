---
title: SAML allkirjastamise probleemide tõrkeotsing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692910"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="79616-102">SAML allkirjastamise probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="79616-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="79616-103">SAML allkirjastamise serdi probleemi lahendamiseks tehke järgmised Soovitatavad toimingud.</span><span class="sxs-lookup"><span data-stu-id="79616-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="79616-104">Kui lisate ettevõtte rakenduse, mis toetab SSO-d, loob Azure serdi, mida nimetatakse [SAML allkirjastamise serdiks](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="79616-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="79616-105">Sellel serdil on tähtaeg 3 aastat.</span><span class="sxs-lookup"><span data-stu-id="79616-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="79616-106">Serdi aegumiskuupäeva muutmiseks lugege teemat [Föderatsiooni serdi aegumiskuupäeva kohandamine ja selle ümberpaigutamine uuele serdile](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="79616-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="79616-107">Azure kasutab seda serti rakenduse nõutud SAML märkide allkirjastamiseks ja saadab selle eduka SSO taotlusele.</span><span class="sxs-lookup"><span data-stu-id="79616-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="79616-108">Selle lõpule viimiseks Laadige alla Azure ' i portaalist sert ja saatke see SSO protsessi lõpuleviimiseks rakenduse tarnijale.</span><span class="sxs-lookup"><span data-stu-id="79616-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="79616-109">Kui toiming on lõpule jõudnud, usaldab rakendus selle serdi ja kõik selle serdi allkirjastatud SAML kinnitatakse rakendusega.</span><span class="sxs-lookup"><span data-stu-id="79616-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="79616-110">Kui see sert aegub, looge uus sert, värskendage see rakenduse tarnijaga ja seejärel aktiveerige see Azure ' i poolel.</span><span class="sxs-lookup"><span data-stu-id="79616-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="79616-111">Lisateavet leiate teemast [varsti aegunud serdi pikendamine](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="79616-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="79616-112">Kui sert aegub, siis kasutajat ei blokeerita.</span><span class="sxs-lookup"><span data-stu-id="79616-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="79616-113">[Saate lisada](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) meiliaadressid enne praeguse serdi aegumist saadud teatiste jaoks.</span><span class="sxs-lookup"><span data-stu-id="79616-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="79616-114">Step-4 on valikuline.</span><span class="sxs-lookup"><span data-stu-id="79616-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="79616-115">Saate muuta rakenduse SAML serdi allkirjastamise suvandeid ja serdi allkirjastamise algoritmi.</span><span class="sxs-lookup"><span data-stu-id="79616-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="79616-116">Lisateavet leiate teemast [serdi allkirjastamise suvandite ja allkirjastamise algoritmi muutmine](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="79616-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
