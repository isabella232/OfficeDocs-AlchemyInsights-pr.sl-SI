---
title: Dovoljenja za API in soglasja
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974994"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="c2d66-102">Dovoljenja za API in soglasja</span><span class="sxs-lookup"><span data-stu-id="c2d66-102">API permissions and consent</span></span>

<span data-ttu-id="c2d66-103">Programi, ki se integrirajo s platformo Microsoft Identity, spremljajo model avtorizacije, ki uporabnikom in skrbnikom omogoča nadzor nad tem, kako je mogoče dostopati do podatkov.</span><span class="sxs-lookup"><span data-stu-id="c2d66-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="c2d66-104">Izvajanje modela odobritve je bilo posodobljeno na končni točki Microsoftove platforme za identiteto.</span><span class="sxs-lookup"><span data-stu-id="c2d66-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="c2d66-105">Spreminja, kako mora program delovati z Microsoftovo platformo Identity.</span><span class="sxs-lookup"><span data-stu-id="c2d66-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="c2d66-106">[Dovoljenja in soglasje v končni točki Microsoftovega izhodišča identitete](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) so osnovni pojmi tega modela odobritve, vključno z obsegi, dovoljenji in soglasjem.</span><span class="sxs-lookup"><span data-stu-id="c2d66-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="c2d66-107">[Okvir soglasja Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) omogoča preprosto razvijanje spletnih in odjemalskih programov za več najemnikov.</span><span class="sxs-lookup"><span data-stu-id="c2d66-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="c2d66-108">Ti programi dovoljujejo vpis s strani uporabniških računov iz strežnika Azure AD najemnika, ki je drugačen od tistega, v katerem je program registriran.</span><span class="sxs-lookup"><span data-stu-id="c2d66-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="c2d66-109">Poleg svojih spletnih vmesnikov API lahko tudi potrebujejo dostop do spletnih vmesnikov API, kot je Microsoft Graph API (za dostop do storitev Azure AD, InTune in storitve Microsoft 365) in drugih API-jev Microsoftovih storitev.</span><span class="sxs-lookup"><span data-stu-id="c2d66-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

