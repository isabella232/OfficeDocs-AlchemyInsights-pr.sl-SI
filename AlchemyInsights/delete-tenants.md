---
title: Izbriši najemnika
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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993909"
---
# <a name="delete-tenant"></a>Izbriši najemnika

Če želite izbrisati Azure AD, poskrbite za to:
- Ste globalni skrbnik v imeniku.
- NISTE vpisani z računom, ki ima privzeti imenik, kot je contoso.onmicrosoft.com v račun za vpis, na primer admin@contoso.onmicrosoft.com.
- Pred brisanjem odstranite vse aktivne aplikacije v imeniku. Če želite odstraniti aktivne aplikacije, se pomaknite na Registracije aplikacij in odstranite obstoječe aplikacije.
- Za nobeno od storitev Microsoft Online, kot je Microsoft Azure, Office 365 ali Azure AD Premium v imeniku ni aktivne naročnine. Prenesite svoje naročnine ali pospešite preklic aktivnih naročnin prek podpore in obračunavanja za Azure. Preberite več o preklicu naročnin na Office 365 Azure in Azure. Če želite navodila za povezovanje ali dodajanje obstoječe naročnine najemniku, glejte Povežite ali dodajte naročnino na Azure najemniku [imenika Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Aktivna licenca ni na voljo. Če želite odstraniti licence, glejte [Kako odstraniti naročnino za odstranitev licence.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- V imeniku ni drugih aktivnih uporabnikov, razen sebe kot globalni skrbnik, ko poskušate izbrisati Imenik Azure AD. Odstranite vse druge aktivne uporabnike in odstraniti boste morali tudi morebitne odvisnosti od imena domene po meri v najemniku, na primer uporabnike, ustvarjene s storitvijo admin@contoso.com.

Če želite več podrobnosti o tem, kako:
- Izbrišite »Azure Active Directory« ali »naročnino«, glejte [Brisanje Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Odstranjevanje programov v imeniku, glejte [Odstranjevanje programov.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
