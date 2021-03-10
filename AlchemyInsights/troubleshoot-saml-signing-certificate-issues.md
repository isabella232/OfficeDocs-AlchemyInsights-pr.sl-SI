---
title: Odpravljanje težav z SAML podpisom potrdil
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
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694450"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="86596-102">Odpravljanje težav z SAML podpisom potrdil</span><span class="sxs-lookup"><span data-stu-id="86596-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="86596-103">Če želite odpraviti težavo s podpisom potrdila SAML, izvedite te priporočene korake:</span><span class="sxs-lookup"><span data-stu-id="86596-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="86596-104">Ko dodate program za podjetja, ki podpira SSO, bo Azure ustvaril potrdilo, ki se imenuje [SAML podpisno potrdilo](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="86596-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="86596-105">To potrdilo ima rok trajanja 3 leta.</span><span class="sxs-lookup"><span data-stu-id="86596-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="86596-106">Če želite spremeniti datum poteka potrdila, si oglejte [prilagajanje datuma poteka za potrdilo o poteku veljavnosti potrdila o poteku in ga prepeljite v novo potrdilo](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="86596-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="86596-107">Azure bo s tem potrdilom podpisal žetone SAML, ki jih zahteva aplikacija, in ga poslal v program za uspešno SSO.</span><span class="sxs-lookup"><span data-stu-id="86596-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="86596-108">Če želite, da se to dokonča, prenesite potrdilo iz portala Azure in ga pošljite prodajalcu programov, da dokončate postopek SSO.</span><span class="sxs-lookup"><span data-stu-id="86596-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="86596-109">Ko je ta postopek končan, bo aplikacija zaupala temu potrdilu in vsi SAML žetoni, ki jih podpiše to potrdilo, bodo sprejeli program.</span><span class="sxs-lookup"><span data-stu-id="86596-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="86596-110">Če to potrdilo poteče, ustvarite novo potrdilo, ga posodobite na prodajalca aplikacij in ga nato naredite na strani Azure Side.</span><span class="sxs-lookup"><span data-stu-id="86596-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="86596-111">Če želite več informacij, glejte [podaljšanje potrdila, ki bo kmalu potekla](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="86596-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="86596-112">Če potrdilo poteče, uporabnik ne bo blokiran.</span><span class="sxs-lookup"><span data-stu-id="86596-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="86596-113">[Dodajanje e-poštnega naslova za obvestila](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) , ki bodo prejeta, preden potek trenutnega potrdila poteče.</span><span class="sxs-lookup"><span data-stu-id="86596-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="86596-114">Step-4 je izbirna ena.</span><span class="sxs-lookup"><span data-stu-id="86596-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="86596-115">Spremenite možnosti podpisa potrdila programa SAML in algoritem za podpis potrdila.</span><span class="sxs-lookup"><span data-stu-id="86596-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="86596-116">Če želite več informacij, glejte [Spreminjanje možnosti podpisovanja potrdil in algoritma za podpis](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="86596-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

