---
title: Težave s soglasjem skrbnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901512"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="923c6-102">Težave s soglasjem skrbnika</span><span class="sxs-lookup"><span data-stu-id="923c6-102">Admin consent issues</span></span>

1. <span data-ttu-id="923c6-103">Omogočite [potek dela](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) skrbnika, če želite uporabnikom omogočiti, da zahtevajo skrbniško odobritev neposredno na zaslonu soglasja.</span><span class="sxs-lookup"><span data-stu-id="923c6-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="923c6-104">Če vi ali uporabniki aplikacije vidijo nepričakovane napake med postopkom odobritve, si oglejte ta članek navodila za odpravljanje težav: [Nepričakovana napaka pri izvajanju dovoljenja za program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="923c6-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="923c6-105">Več informacij o [soglasju skrbnika na platformi Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), kako deluje [poziv za privolitev](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) in kako [ovrednotiti zahtevo za odobritev skrbnika za celotno najemnika](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="923c6-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="923c6-106">Programi, ki se integrirajo s platformo Microsoft Identity, spremljajo model avtorizacije, ki uporabnikom in skrbnikom omogoča nadzor nad tem, kako je mogoče dostopati do podatkov.</span><span class="sxs-lookup"><span data-stu-id="923c6-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="923c6-107">Izvajanje modela za avtorizacijo je bilo posodobljeno na končni točki Microsoftovega izhodišča za identiteto in spremeni, kako mora program delovati z Microsoftovo platformo Identity.</span><span class="sxs-lookup"><span data-stu-id="923c6-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="923c6-108">Če želite pregled tega modela odobritve, vključno s obsegi, dovoljenji in soglasjem, si oglejte [dovoljenja in soglasje v končni točki za Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) .</span><span class="sxs-lookup"><span data-stu-id="923c6-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>