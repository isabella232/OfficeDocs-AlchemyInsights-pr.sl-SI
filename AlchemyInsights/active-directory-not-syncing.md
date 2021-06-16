---
title: Imenik Active Directory se ne sinhronizira
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930991"
---
# <a name="active-directory-not-syncing"></a>Imenik Active Directory se ne sinhronizira

Če prejemate napake pri sinhronizaciji, na primer »ni nedavne sinhronizacije«, ali pa opazite stanje sinhronizacije imenika v skrbniškem portalu za Office pravi »Zadnja sinhronizacija je bila sinhronizirana pred več kot 3 dnevi«, ima morda AADConnect nepravilne nastavitve ali nezadostna dovoljenja za izvajanje sinhronizacije.  

Če znova namestite AADConnect s hitrimi nastavitvami, boste težavo morda lahko hitro odpravili:

1. [Prenesite najnovejšo različico programa AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Upoštevajte navodila za hitro namestitev.](/azure/active-directory/hybrid/how-to-connect-install-express)

Storitev Azure AD Connect mora biti nameščena v strežniku Windows Server 2012 ali novejši različici. Ta strežnik mora biti pridružena domena in je lahko krmilnik domene oziroma članski strežnik. Za celoten seznam zahtev in Povezovalnik imenika Azure AD si oglejte Zahteve za imenik [Azure AD Povezovalnik](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Če želite več informacij o računih storitve AADConnect, glejte [Azure AD Povezovalnik: Računi in dovoljenja.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
