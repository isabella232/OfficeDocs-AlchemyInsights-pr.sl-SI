---
title: Odpravljanje težav z uporabniškimi težavami
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
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901338"
---
# <a name="announcements"></a>Obvestila

Upoštevajte navodila za Google o preverjanju združljivosti za preverjanje, ali so vaši programi prizadeti. V storitvi Google je na voljo navodila https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Zagotovite, da pri vpisu uporabnikov s storitvijo Google računi za uporabnike uporabite spletni pogled sistema ali sistemskega brskalnika. Če želite več informacij, glejte [težave pri vpisu v program le z brskalnikom Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Ne morem ustvariti novega uporabnika v imeniku Azure AD Directory**

Če želite odpraviti težavo, ko ne morete ustvariti novega uporabnika v storitvi Azure AD, upoštevajte te korake:

1. Zagotovite, da imate dovoljenje za ustvarjanje novega standardnega uporabnika. V storitvi Azure Active Directory (AD) lahko ustvari novega standardnega uporabnika le globalni skrbnik ali skrbnik uporabnika. Če niste v eni od teh vlog, prosite skrbnika, da vas doda v eno od teh vlog, ali pa ustvarite nov uporabniški račun.
2. Zagotovite, da je uporabniško ime v domeni, ki je preverjena v storitvi Azure AD. Če nimate preverjenih imen domen po meri v storitvi Azure AD, lahko uporabite začetno domeno storitve Azure AD, ki se konča z *. onmicrosoft.com.
3. Zagotovite, da je uporabniško ime v domeni, ki ni Združeno do storitve Azure AD iz OGLASa na mestu uporabe. Uporabnikov ni mogoče dodati v oblak z imeni domen, ki so Združene od na mestu uporabe.
4. Zagotovite, da noben drug uporabnik ali stik že nima uporabniško ime, ki ga želite dodeliti novemu uporabniku. Uporabniška imena morajo biti enolična v storitvi Azure AD.
5. Glejte [vloge za AZURE ad in skrbnike](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za vaš oglas Azure.
6. Glejte [imena domen](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) za svoj oglas Azure.
7. Preglejte [dnevnike nadzora](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) , če si želite ogledati podrobnejše informacije o nedavno ustvarjenem ali izbrisanem uporabniku, kot je bil izveden postopek in kdaj.
8. Če želite več informacij o dodajanju novih uporabnikov, [si oglejte Uporaba portala Azure za ustvarjanje novega uporabnika v storitvi AZURE ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Če želite več informacij o dovoljenjih skrbniških vlog v storitvi Azure AD, glejte [skrbniške vloge za AZURE ad](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Če želite več informacij o ustvarjanju uporabnika s storitvijo Azure AD PowerShell, glejte [AZURE ad PowerShell za ustvarjanje novega uporabnika](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Težave s samopostrežnim vpisom**

Če želite odpraviti težave z vpisom v samopostrežne storitve, izvedite te korake:

1. Če želite uporabiti samopostrežno prijavo z vašimi programi, najprej omogočite prijavo za samostoritev za najemnika. 
2. Če želite omogočiti aplikacijo, ki podpira samopostrežno prijavo, jo dodajte v svoj potek uporabnika. Ko se naslednjič vrnete na stran za prijavo za ta program, se prikaže možnost **_brez računa? Ustvarite eno!_* _. S tem se zažene postopek prijave samopostrežne storitve.
3. Če želite več informacij o tem, kako lahko uporabite samopostrežno prijavo, da zapolnite organizacijo v storitvi Azure AD, glejte [samopostrežni vpis v storitev AZURE ad](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Ko povežete uporabniški tok z enim ali več programi, bodo uporabniki, ki obiščejo to aplikacijo, lahko prijavili in pridobili račun za goste z možnostmi, ki so konfigurirani v toku uporabnika. Če želite več informacij o vpisu in pridobivanju računa za goste, si lahko uporabniki ogledajo [samopostrežno prijavo za gostujoče uporabnike](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Težava pri povabilu zunanjega uporabnika**

Če želite odpraviti težave, ki se nanašajo na povabilo zunanjega uporabnika, izvedite ta korak:

Zagotovite, da pošljete povabilo uporabnika na e-poštni naslov, ki se ujema z imenom, s katerim se uporabnik prijavi. Če pošljete povabilo na e-poštni naslov uporabnika proxy, ga uporabnik ne more odkupiti. Če želite več informacij, glejte dokumentacija o storitvi [AZURE ad B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Uporabniku ne morem dodeliti licenc**

Če želite odpraviti težave z dodeljevanjem licenc uporabniku, izvedite te korake:

1. Če želite upravljati uporabniške licence, zagotovite, da uporabite račun z eno od zahtevanih skrbniških vlog: globalni skrbnik, skrbnik licence ali skrbnik uporabnika. Vlogo uporabnika lahko preverite na zavihku» **vloga imenika** «na rezilu uporabnika.
2. Če uporabljate portal Azure in dodelitev licence ni uspešna, kliknite obvestilo v zgornjem desnem kotu. S tem odprete rezilo s podrobnostmi o tem, kaj je šlo narobe. V večini primerov je to dovolj, da razumete in odpravite težavo.
3. Preden lahko licenco dodelite uporabniku, zagotovite, da je lastnost **lokacija uporabe** nastavljena za uporabnika. Preverite, ali ima uporabnik nastavljeno lastnost tako, da si ogleda zavihek **profila** na rezilu uporabnika.
4. Zagotovite, da je za izdelek, ki ga poskušate dodeliti, dovolj razpoložljivih licenc. Število razpoložljivih licenc v portalu Azure najdete na spletnem mestu [Azure Active Directory – > licence – > vse izdelke](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Uporabnik lahko že ima drugo licenco, katere storitve so v sporu s tistimi v novi licenci, ki jo poskušate dodeliti. Če ima uporabnik na primer omogočeno storitev Exchange Online (paket 1), ne boste mogli dodeliti licence za Exchange Online (paket 2). Onemogočite eno od storitev, če želite omogočiti novo dodelitev licence. Če uporabljate portal Azure ali ukaze» cmdlet «za PowerShell, je na strani s **podrobnostmi o težavi** seznam določenih storitev, ki povzročajo spor.
6. Če poskušate odstraniti licenco in ki ni uspešna, ima uporabnik morda druge licence s storitvami, ki so odvisne od storitev, ki jih skušate odstraniti. Če uporabljate portal Azure ali ukaze» cmdlet «za PowerShell, se prikaže sporočilo o napaki, ki vsebuje določene storitve, ki imajo odvisnosti.
7. Če želite razumeti, zakaj je bila licenca dodana/odstranjena iz uporabnika (na primer, kdo v vaši organizaciji je morda spremenil), preverite dnevnike nadzora. Če želite prikazati vse spremembe, vključno z» igralcem «, ki jih je opravil, nastavite filter na **licence** .
8. Če uporabljate Exchange Online, so nekateri uporabniki v najemniku morda nepravilno konfigurirani z isto vrednostjo naslova strežnika proxy. V teh primerih se lahko prikažejo splošna sporočila o napakah, ko postopek licence ne uspe. V [tem članku](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) je več informacij o tej težavi, vključno s podatki o [povezovanju s storitvijo Exchange Online z uporabo oddaljenega PowerShella](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Če želite ugotoviti, kateri uporabniki v najemniku vsebujejo isti naslov strežnika proxy, izvedite ta ukaz» cmdlet «Exchange Online:

Zagon

Get-Recipient | Kje je {$ _. EmailAddresses – Match <user principal name> } | Ime fL, RecipientType, emailaddresss





