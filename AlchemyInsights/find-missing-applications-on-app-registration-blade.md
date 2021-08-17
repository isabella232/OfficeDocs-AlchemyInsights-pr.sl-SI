---
title: Find missing applications on App Registration blade
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057118"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Find missing applications on App Registration blade

1. Programov ni mogoče najti na portalu za registracijo aplikacije.

    Če je program program z več najemniki in je bil registriran v drugem najemniku, ne bo prikazan v razdelku Registracija aplikacije. Lahko pa ga najdete v razdelku Rega aplikacije za podjetja, ko je dostop do njega (po soglasju) in glavno ime storitve ustvarjeno v vašem najemniku. Če želite več informacij, [glejte & glavna podjetja storitve v Imeniku Azure AD – Microsoftova platforma za identitete.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Programov si ni mogoče ogledati v reji registracije programov, čeprav ste skrbnik.

    Prepričajte se, da ste v pravem imeniku na portalu Azure.
3. Moj program ni naveden v razdelku re blade enterprise Applications, vendar se prikaže, ko poizvednem po ukazu PowerShell.

    Ko aplikacijo izbrišete iz portala Azure, ta včasih ni več prikaže v portalu, vendar morda ni bila v celoti izbrisana. Če želite več informacij, si oglejte:
    - Seznam izbrisanih aplikacij lahko pridobite in z ukazom Powershell prikažete program na seznamu: **Get-AzureADDeletedApplication.** Če želite izvedeti več, [glejte Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Če želite popolnoma odstraniti aplikacijo, lahko poskusite to v lupini PowerShell: **Remove-AzureADApplication -ObjectId**. Če želite izvedeti več, [glejte Odstranjevanje storitve AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Lahko pa poskusite obnoviti izbrisano aplikacijo s tem ukazom Powershell: **Restore AzureADDeletedApplication -ObjectId**. Če želite izvedeti več, [glejte Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. V novem najemniku Azure ni mogoče najti seznama vseh vnaprej nameščenih poslovnih aplikacij.

    V imeniku Azure AD privzeto niso nameščene vnaprej nameščene poslovne aplikacije. Aplikacijo morate dodati ročno iz možnosti »Nova aplikacija« tako, da jo po brskanjem poište iz galerije Azure AD ali dodate aplikacijo, ki ni iz galerije. Če želite izvedeti več, [glejte Vodnik za hitri začetek: dodajanje programa v najemnika Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Če ste globalni skrbnik, lahko do aplikacij preprosto dostopate z zaganjalnika [Microsoft 365 programov.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Mojih aplikacij ni mogoče najti na portalu »Moji programi«.

    Prepričajte se, da programi niso skriti na strani zbirke mojih programov. Če želite izvedeti več, glejte [Zbirke (predogled) na portalu »Moje aplikacije« – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Če želite zagnati aplikacije na portalu »Moje aplikacije& poiščite aplikacije na [portalu »Moje aplikacije« – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Aplikacija Mover po namestitvi ni prikazana v reži programa Enterprise Applications.

    Program »Office 365 Mover« je program z več najemniki, ki ga ni treba dodati v AAD z razdelkom Aplikacije galerije v razdelku Registracija programa podjetja. Če Office 365 aplikacijo Mover, se preprosto vpišite v aplikacijo in prosite za soglasje uporabnika za dovoljenja. Ko uporabnik da soglasje, se ta aplikacija samodejno doda v najemnika z e-poštnim ID-jem, ki ste ga prijavili.

    Po vpisu v aplikacijo boste lahko našli vnos tega programa pod re bladeom programa za podjetja v AAD. Aplikacijo lahko poiščete tako, da vnesete polno ime, na primer »Office 365 Mover«, ali pa preprosto poiščete »Office«, program pa naj bo seznam. Če želite izvedeti več, Office 365 Mover pravi, da je že nameščen, vendar ni naveden v [galeriji programov za podjetja.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. Hitri začetek: Oglejte si seznam aplikacij, ki za upravljanje identitet uporabljajo najemnika [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) in vam pokaže, kako si ogledate aplikacije, znane tudi kot aplikacije, ki so že nastavljene za uporabo najemnika imenika Azure AD kot ponudnika identitete (IdP).
9. [Odpravite pogoste težave z dodajanjem ali odstranjevanjem](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) programa v Azure Active Directory, da boste lažje razumeli pogoste težave, s katerimi se srečujejo osebe z Azure Active Directory.
