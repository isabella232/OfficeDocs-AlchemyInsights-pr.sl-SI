---
title: Odpravljanje težav z dostopom do zavrnjenih sporočil
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767679"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="b567a-102">Odpravljanje težav z dostopom do sporočil v skrbniškem središču za SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="b567a-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="b567a-103">Če prejmete sporočilo o zavrnjenem dostopu ob poskusu brskanja v skrbniškem središču za SharePoint/OneDrive, se prepričajte, da ste [uporabniku dodelili licenco](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="b567a-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="b567a-104">Če ima uporabnik licenco, se prepričajte, da jim je [dodeljena skrbniška vloga](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , ki lahko dostopa do skrbniških centrov.</span><span class="sxs-lookup"><span data-stu-id="b567a-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="b567a-105">Do te težave lahko pride tudi, ko je uporabnik izbrisan in znova ustvarjen z istim glavnim imenom uporabnika (UPN).</span><span class="sxs-lookup"><span data-stu-id="b567a-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="b567a-106">Nov račun je ustvarjen z uporabo drugega PUID (ID Passporta Unique).</span><span class="sxs-lookup"><span data-stu-id="b567a-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="b567a-107">Ko uporabnik poskuša dostopati do zbirke mest ali njihove OneDrive, ima uporabnik nepravilen PUID.</span><span class="sxs-lookup"><span data-stu-id="b567a-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="b567a-108">Drugi scenarij vključuje sinhronizacijo imenika z organizacijsko enoto imenika Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="b567a-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="b567a-109">Če so uporabniki že vpisani v SharePoint, nato pa so premaknjeni v drug OU in znova sinhronizirani s storitvijo SharePoint, lahko ta težava pride do te težave.</span><span class="sxs-lookup"><span data-stu-id="b567a-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="b567a-110">To težavo odpravite tako, da obnovite prvotni UPN s koraki v članku, [obnovite uporabnika v programu Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="b567a-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="b567a-111">Opomba: Če v skrbniškem središču za OneDrive ali SharePoint ni na voljo več uporabnikov, ki so prej imeli dostop, je morda prišlo do začasne težave s storitvijo.</span><span class="sxs-lookup"><span data-stu-id="b567a-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="b567a-112">[Preverite nadzorno ploščo za stanje storitve](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b567a-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


