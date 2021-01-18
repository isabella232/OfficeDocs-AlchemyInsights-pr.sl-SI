---
title: Konfiguracija storitve Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885687"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="0dfc9-102">Ne morete omogočiti ZVOČNIh naprav – DS ali uvedbe ni mogoče</span><span class="sxs-lookup"><span data-stu-id="0dfc9-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="0dfc9-103">Če želite odpraviti težavo z domensko storitvijo Azure AD (ZVOČNa-DS), ki ni omogočena ali ni bila uvedena, izvedite te korake:</span><span class="sxs-lookup"><span data-stu-id="0dfc9-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="0dfc9-104">Če uporabljate že obstoječo navidezno omrežje, potrdite NSG za pravila, ki blokirajo vrata, potrebna za sinhronizacijo v storitvi ZVOČNa-DS v portalu https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="0dfc9-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="0dfc9-105">Preverite, ali je odgovor na sporočilo o napaki v tem vodniku za odpravljanje težav, ki je na voljo  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="0dfc9-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="0dfc9-106">Poskusite uporabiti domenske storitve Azure AD v novem navideznem omrežju.</span><span class="sxs-lookup"><span data-stu-id="0dfc9-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="0dfc9-107">Navodila za začetek vodnika za uvajanje ZVOČNIh [storitev](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)</span><span class="sxs-lookup"><span data-stu-id="0dfc9-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="0dfc9-108">Če imate težave z uvajanjem domen v storitvi Azure AD Services, glejte [Odpravljanje težav z domenami storitve AZURE ad](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , da odpravite pogoste napake, s katerimi lahko znova začnete delati.</span><span class="sxs-lookup"><span data-stu-id="0dfc9-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="0dfc9-109">**Ne morete onemogočiti ZVOČNIh-DS**</span><span class="sxs-lookup"><span data-stu-id="0dfc9-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="0dfc9-110">ZVOČNa-DS ne more biti začasno ustavljena.</span><span class="sxs-lookup"><span data-stu-id="0dfc9-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="0dfc9-111">Če želite prenehati uporabljati upravljano domeno, jo morate izbrisati.</span><span class="sxs-lookup"><span data-stu-id="0dfc9-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="0dfc9-112">Če želite izbrisati upravljano domeno, si oglejte [brisanje storitve v storitvi zvočna domena](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="0dfc9-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



