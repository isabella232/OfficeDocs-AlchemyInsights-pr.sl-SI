---
title: Skrivnost odjemalca za registracijo aplikacije ali težave s potrdilom
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405332"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="3e140-102">Skrivnost odjemalca za registracijo aplikacije ali težave s potrdilom</span><span class="sxs-lookup"><span data-stu-id="3e140-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="3e140-103">Ali skrivnost odjemalca aplikacije poteče?</span><span class="sxs-lookup"><span data-stu-id="3e140-103">Application client secret expiring?</span></span>

<span data-ttu-id="3e140-104">Ne glede na to, kako je bila registrirana aplikacija ustvarjena, ne glede na to, ali uporabljate standardni postopek registracije v portalu za registracijo aplikacij ali če je bilo glavno ime storitve v vašem najemniku ustvarjeno s soglasjem aplikacije, bo treba ustvariti novo skrivnost odjemalca pred potekom trenutne in posodobljene v povezani kodi aplikacije.</span><span class="sxs-lookup"><span data-stu-id="3e140-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="3e140-105">Najdaljše obdobje veljavnosti je 2 leti.</span><span class="sxs-lookup"><span data-stu-id="3e140-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="3e140-106">Kot opomnik, je treba skrivno vrednost zabeležiti, saj ne bo več vidna, ko zapustite stran Registracije aplikacij v portalu.</span><span class="sxs-lookup"><span data-stu-id="3e140-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="3e140-107">Če želite več informacij, glejte [Vodnik za hitri začetek: registrirajte](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) program v Microsoftovi platformi identitete in Najboljše prakse za [Microsoftovo platformo identitete.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="3e140-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="3e140-108">Če želite izvedeti več, [glejte Ustvarjanje aplikacije Azure AD & glavnem imenu storitve na portalu – Microsoftova platforma za identitete.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="3e140-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
