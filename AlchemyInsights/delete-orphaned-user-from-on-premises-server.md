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
# <a name="delete-orphaned-user-from-on-premises-server"></a>Izbris osirotelega uporabnika iz krajevnega strežnika

Če želite odstraniti osirotelega uporabnika, sledite tem korakom:

1. Vsilite sinhronizacijo imenika tako, da upoštevate navodila v [Kaj je hibridna identiteta s storitvijo Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Če želite preveriti sinhronizacijo imenika, glejte [Kaj je hibridna identiteta s storitvijo Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Če sinhronizacija deluje pravilno, vendar se brisanje predmeta imenika Active Directory ne razširi na Azure AD, ročno odstranite osirotelega predmeta z uporabo enega od teh modulih ukazov Azure Active Directory za ukaze» cmdlet «lupine Windows PowerShell:

    Odstrani-MsolContact  
    Odstrani-MsolGroup  
    Odstrani-MsolUser

    Če želite na primer odstraniti osiroteli ID uporabnika john.smith@contoso.com, ki je bil prvotno ustvarjen z uporabo sinhronizacije imenika, zaženite ukaz» cmdlet «:

    Premestitev-MsolUser – UserPrincipalName John.Smith@Contoso.com