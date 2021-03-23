---
title: Težave z upravljanjem uporabnikov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037509"
---
# <a name="user-management-issues"></a>Težave z upravljanjem uporabnikov

**Kaj se zgodi s trenutnimi dodeljenimi uporabniki programa, če onemogočim» zahtevano dodelitev uporabnika «(nastavitev te lastnosti na ne)?**

Onemogočanje **zahteve za dodelitev uporabnika** ne vpliva na trenutno dodeljene uporabnike. Onemogočanje te lastnosti bo le vsem uporabnikom omogočilo dostop do programa. Vsi navedeni uporabniki in Uporabniki, ki so dodeljeni skupinam v programu, bodo še vedno veljavni.

- Če želite omejiti program na določen nabor uporabnikov, glejte – [omejite aplikacijo AZURE ad v nabor uporabnikov – Microsoftova platforma za identiteto | Microsoft docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Če želite uporabnikom in skupinam dodeliti programe za podjetja v storitvi Azure Active Directory (Azure AD), ki so na portalu Azure ali z uporabo lupine PowerShell, glejte [upravljanje dodelitve uporabnika za program v imeniku Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Če želite dodeliti dovoljenja za ustvarjanje in upravljanje programov, glejte [dodeljevanje skrbniških dovoljenj za upravljanje programov – AZURE ad | Microsoft docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Skrivanje določenih aplikacij za podjetja od uporabnikov** – uporabite te korake, da skrijete vse aplikacije Microsoft 365 v podoknu **MyApps** . Programi bodo še vedno vidni v portalu za Office 365.

 1. Vpišite se v portal Azure kot globalni skrbnik za vaš imenik. 
 2. Izberite **Azure Active Directory**. 
 3. Izberite **Uporabniki**. 
 4. Izberite **nastavitve uporabnika**. 
 5. V razdelku **aplikacije Enterprise** kliknite **upravljanje, kako končni uporabniki zaženejo in si ogledajo svoje aplikacije**. 
 6. **Uporabniki si lahko ogledajo le programe sistema office 365 na portalu za office 365**, kliknite **da**. 
 7. Kliknite **Shrani**. 
 8. Če želite več informacij, glejte [skrivanje aplikacije Enterprise iz izkušnje uporabnikov v storitvi AZURE ad | Microsoft docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Če za številne organizacije ponudite programsko opremo kot storitev (SaaS), lahko program konfigurirate tako, da sprejema vpise iz katerega koli imenika Azure Active Directory (Azure AD). Ta konfiguracija se imenuje» ustvarjanje več najemnikov aplikacije «. Uporabniki v katerem koli najemniku v storitvi Azure AD se bodo lahko prijavili v vašo aplikacijo po tem, ko bodo privolili k uporabi svojega računa v aplikaciji. Če želite več informacij, glejte [Ustvarjanje programov, ki se vpišejo v uporabnike storitve AZURE ad – Microsoftova platforma za identiteto | Microsoft docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Kako lahko končni uporabnik dostopa do aplikacije, ko je dodeljena programu?**

Vsak program v rezilu aplikacije Enterprise ima povezavo za končne uporabnike za dostop. Uporabniki lahko dostopajo do programa prek portala **Myapps** na preprost način.

- **Ali želite izvedeti, katere aplikacije in vrsto programov uporabljajo Uporabniki?**

Poročila o vpisu lahko prenesete v zadnjih 30 dneh od **portal.azure.com > Azure Active directory> Signins> prenos poročil**.

- Naučite se [dodeliti soglasje skrbnika za široko uporabo](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) in [konfigurirajte, kako končni uporabniki soglašajo z aplikacijami](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Razumete, [Kako soglasje deluje](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) in [upravlja soglasje za aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


