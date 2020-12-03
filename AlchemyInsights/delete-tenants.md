---
title: Brisanje najemnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564880"
---
# <a name="delete-tenant"></a>Brisanje najemnika

Če želite izbrisati oglas Azure, zagotovite:
- Ste globalni skrbnik v imeniku.
- Niste vpisani z računom, ki ima privzeti imenik, kot je contoso.onmicrosoft.com, v računu, kot je na primer admin@contoso.onmicrosoft.com.
- Pred brisanjem odstranite vse aktivne aplikacije v imeniku. Če želite odstraniti aktivne aplikacije, se pomaknite do registracij programov in odstranite obstoječe aplikacije.
- Ni aktivnih naročnin za vse Microsoftove spletne storitve, kot je Microsoft Azure, Office 365 ali Azure AD Premium, ki je povezan v imeniku. Prenesite naročnine ali pospešite preklic aktivnih naročnin prek storitve Azure support in obračunavanje. Preberite več o tem, kako preklicati naročnine na Office 365 in Azure. Če želite navodila za združevanje ali dodajanje obstoječe naročnine najemniku, [si oglejte povezovanje ali dodajanje naročnine na AZURE ad najemniku](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Ni aktivne licence. Če želite odstraniti licence, si oglejte [Kako odstranite naročnino, da odstranite licenco](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Pri poskusu brisanja Azure AD ni nobenega drugega aktivnega uporabnika v imeniku poleg samega sebe kot globalnega skrbnika. Odstranite vse druge aktivne uporabnike, zato je treba odstraniti tudi vse odvisnosti v imenu domene po meri v najemniku, kot so uporabniki, ustvarjeni z admin@contoso.com.

Če želite več podrobnosti o tem, kako:
- Izbrišite» imenik Azure Active Directory «ali» naročnina «, glejte [brisanje imenika Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Če želite odstraniti aplikacije v imeniku, glejte [odstranjevanje programov](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
