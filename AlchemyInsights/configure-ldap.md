---
title: Konfiguracija protokola LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885578"
---
# <a name="configure-ldap"></a><span data-ttu-id="699f2-102">Konfiguracija protokola LDAP</span><span class="sxs-lookup"><span data-stu-id="699f2-102">Configure LDAP</span></span>

<span data-ttu-id="699f2-103">Če želite konfigurirati protokol LDAP, naredite to:</span><span class="sxs-lookup"><span data-stu-id="699f2-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="699f2-104">Preverite stanje domene na [portalu Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="699f2-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="699f2-105">Zagotovite, da je na voljo veljavna naročnina na Azure AD in je omogočena storitev Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="699f2-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="699f2-106">Potrdilo, ki je zahtevano za omogočanje varnega LDAP, mora biti pridobljeno iz zaupanja vrednega javnega overovitelja ali pa je samopodpisano potrdilo.</span><span class="sxs-lookup"><span data-stu-id="699f2-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="699f2-107">Zagotovite, da bo potrdilo sledilo zahtevanim [navodilom](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="699f2-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="699f2-108">**Neveljavno potrdilo**</span><span class="sxs-lookup"><span data-stu-id="699f2-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="699f2-109">Če želite obnoviti potrdilo, upoštevajte navodila za ustvarjanje novega potrdila in reupload: [Konfiguriranje protokola LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="699f2-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="699f2-110">Če želite razrešiti znano težavo z varnimi opozorili LDAP v domenskih storitvah storitve Azure Active Directory, glejte [Odpravljanje opozoril LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="699f2-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
