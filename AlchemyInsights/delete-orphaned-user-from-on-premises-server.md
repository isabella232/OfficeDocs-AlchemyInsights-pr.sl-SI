---
title: Izbris osirotelega uporabnika iz krajevnega strežnika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198587"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="092b7-102">Izbris osirotelega uporabnika iz krajevnega strežnika</span><span class="sxs-lookup"><span data-stu-id="092b7-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="092b7-103">Če želite odstraniti osirotelega uporabnika, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="092b7-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="092b7-104">Vsilite sinhronizacijo imenika tako, da upoštevate navodila v [Kaj je hibridna identiteta s storitvijo Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="092b7-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="092b7-105">Če želite preveriti sinhronizacijo imenika, glejte [Kaj je hibridna identiteta s storitvijo Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="092b7-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="092b7-106">Če sinhronizacija deluje pravilno, vendar se brisanje predmeta imenika Active Directory ne razširi na Azure AD, ročno odstranite osirotelega predmeta z uporabo enega od teh modulih ukazov Azure Active Directory za ukaze» cmdlet «lupine Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="092b7-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="092b7-107">Odstrani-MsolContact</span><span class="sxs-lookup"><span data-stu-id="092b7-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="092b7-108">Odstrani-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="092b7-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="092b7-109">Odstrani-MsolUser</span><span class="sxs-lookup"><span data-stu-id="092b7-109">Remove-MsolUser</span></span>

    <span data-ttu-id="092b7-110">Če želite na primer odstraniti osiroteli ID uporabnika john.smith@contoso.com, ki je bil prvotno ustvarjen z uporabo sinhronizacije imenika, zaženite ukaz» cmdlet «:</span><span class="sxs-lookup"><span data-stu-id="092b7-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="092b7-111">Premestitev-MsolUser – UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="092b7-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>