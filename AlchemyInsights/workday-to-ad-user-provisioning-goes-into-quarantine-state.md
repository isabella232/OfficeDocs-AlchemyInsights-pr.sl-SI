---
title: Delovni dan do omogočanja uporabe uporabnika v karanteni
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482904"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="193f0-102">Delovni dan do omogočanja uporabe uporabnika v karanteni</span><span class="sxs-lookup"><span data-stu-id="193f0-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="193f0-103">**Delovni dan za omogočanje uporabe uporabnika v sistemu AD gre v stanje karantene in uporabniki niso ustvarjeni v programu AD**</span><span class="sxs-lookup"><span data-stu-id="193f0-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="193f0-104">Posel za omogočanje uporabe uporabnika v programu AD je šel v stanje karantene in dnevniki nadzora kažejo dogodke izvozne neuspelosti z napako sporočila o napaki **: OperationsError-SvcErr: Prišlo je do napake v operaciji. Za imeniško storitev ni bil konfiguriran noben nadrejeni sklic. Imeniška storitev torej ne more izdajati napotitev predmetov zunaj tega gozda**.</span><span class="sxs-lookup"><span data-stu-id="193f0-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="193f0-105">Ta napaka se običajno prikaže, če vsebnik imenika Active Directory OU ni nastavljen pravilno ali če so na voljo težave z izrazom preslikave izraza, ki se uporablja za **parentDistinguishedName**.</span><span class="sxs-lookup"><span data-stu-id="193f0-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="193f0-106">Preverite privzeti parameter OU za **nove uporabnike** za tipkarske napake.</span><span class="sxs-lookup"><span data-stu-id="193f0-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="193f0-107">Zagotovite, da navedeni OU že obstaja v vašem OGLASu.</span><span class="sxs-lookup"><span data-stu-id="193f0-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="193f0-108">Če v preslikavi atributov uporabljate **parentDistinguishedName** , zagotovite, da je vedno ovrednotena z znanim vsebnikom v domeni oglasa.</span><span class="sxs-lookup"><span data-stu-id="193f0-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="193f0-109">Če želite videti ustvarjeno vrednost, v dnevnikih nadzora preverite dogodek izvoza.</span><span class="sxs-lookup"><span data-stu-id="193f0-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="193f0-110">Če želite več informacij o konfiguriranju delovnega dne za avtomatizirano omogočanje uporabe, glejte [Vadnica: konfiguracija delovnega dne za samodejno omogočanje uporabe uporabnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="193f0-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

