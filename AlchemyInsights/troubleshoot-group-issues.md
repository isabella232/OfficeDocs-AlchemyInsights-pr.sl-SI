---
title: Odpravljanje težav z združevanjem
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714447"
---
# <a name="troubleshoot-group-issues"></a>Odpravljanje težav z združevanjem

**Dodati moram skupino v vlogo Azure AD**

Če želite dodeliti skupino Azure Active Directory (AD) v vlogo Azure AD, naredite to:

1. Ustvarjanje nove skupine – če želite ustvariti novo skupino:

    v. Vpišite se v skrbniško središče za Azure AD s privilegiranim skrbnikom za vloge ali globalnimi skrbniškimi dovoljenji. 
    b. Izberite Azure Active Directory > skupine > vse skupine > novo skupino. 
    c. Ustvarite skupino.

2. Dodelite vlogo skupini bodisi med ustvarjanjem skupine ali ko je skupina ustvarjena.

    v. Če želite skupini dodeliti vlogo v času ustvarjanja skupine, lahko v skupino dodelite vloge preklopnega programa Azure AD in ustvarite skupino.
    b. Če želite skupini dodeliti vlogo, ko je bila ustvarjena, se pomaknite do zavihka dodeljene vloge za novo ustvarjeno skupino in dodelite vlogo skupini.

**Upravljati moram članstvo v skupini, ki je dodeljena funkciji Azure AD**

1. Če želite preprečiti dviganje privilegijev, lahko privzeto le privilegirani skrbnik vloge in globalni skrbnik spremeni članstvo v skupini, ki je dodeljena vlogi. Lahko pa se odločijo, da bodo dodeljene lastniku za to skupino in da prenesejo to opravilo. Če želite več informacij, glejte [Uporaba skupin v oblaku za upravljanje dodelitev vlog v storitvi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Če želite pogosta vprašanja in namige za odpravljanje težav z dodeljevanjem vlog skupinam v storitvi Azure AD, glejte [Odpravljanje težav, dodeljenih skupinam v oblaku](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Dinamične skupine**

1. Če ne najdete vgrajenih atributov uporabnika, zagotovite, da je atribut na seznamu podprtih lastnosti.
2. Če iščete vgrajene atribute naprave, zagotovite, da je atribut na seznamu atributov naprave 
3. Poleg vgrajenih atributov uporabnika in naprave lahko uporabite tudi [atribute pripone](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Ko sinhronizirate atribute pripone iz krajevnega strežnika Windows Server AD ali iz povezave storitve SaaS, morajo biti atributi vidni na spustnem seznamu graditelja pravil. Ime atributa po meri je mogoče najti v imeniku tako, da poizveduje uporabnikov atribut z uporabo lupine PowerShell in išče ime atributa. Te se lahko uporabijo tudi pri konstruiranju pravil v sintaksi pravila.
4. Zagotovite, da ima najemnik ustrezno licenco. Dinamične skupine zahtevajo, da najemnik ima licenco za Azure AD P1 Premium. [Tukaj](https://azure.microsoft.com/pricing/details/active-directory/)lahko dostopate do seznama licenčnih paketov za Azure ad. [Tukaj](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)lahko dostopate do paketov za mobilnost podjetij + varnostne licence.
5. Zagotovite, da je vloga uporabnika, ki ustvarja dinamično skupino, globalni skrbnik, program za InTune, skrbnik skupine ali skrbnik uporabnika.
6. Dovolite, da se skupina zapolni. Odvisno od velikosti najemnika lahko skupina traja največ 24 ur, da se prvič zapolni ali ko se spremeni pravilo.
7. Če želite več informacij, glejte [Ustvarjanje pravil, ki temeljijo na atributih za dinamično članstvo v skupini](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Moram izbrisati skupino**

1. Skupine lahko izbrišete iz imenika z ukazom» cmdlet «Remove-AzureADGroup v modulu Azure AD PowerShell.
2. Preden poskusite izbrisati sinhronizirano skupino v storitvi Azure AD, poskrbite, da boste izbrisali vse dodeljene licence, da se izognete napakam.
3. Če želite več informacij o brisanju skupin, [si oglejte brisanje skupine z dodeljeno licenco](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Obnoviti moram izbrisano skupino**

1. Če je skupina Office 365 izbrisana, jo lahko obnovite le do 30 dni, preden pride do trajnega brisanja. Ko je skupina trajno izbrisana, je ni več mogoče obnoviti. Preberite več o obnavljanju skupin [tukaj](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Ta funkcija ni podprta za varnostne skupine in skupine prejemnikov.
3. Zagotovite, da imate dovoljenje za obnovitev skupine sistema Office 365. Globalni skrbniki, skrbniki skupine, skrbniki uporabniških računov, upravitelji storitev InTune, skrbniki storitve partnerja Tier1 ali tier2 in lastnik skupine lahko obnovijo skupino.
4. Ko je dinamična skupina izbrisana in obnovljena, je videti kot nova skupina in znova izpolnjena glede na pravilo. Ta postopek lahko traja največ 24 ur.
5. Če želite več informacij o obnavljanju izbrisane skupine, glejte [obnovitev izbrisane skupine sistema Office 365 v imeniku Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Konfiguracija pravilnika o poteku veljavnosti skupine**

1. Ta funkcionalnost je podprta le za skupine sistema Office 365 in ne za varnostne skupine in skupine prejemnikov niso podprte.
2. Konfiguracija in uporaba pravilnika o zapadlosti za skupine sistema Office 365 zahteva licenco storitve Azure AD Premium.
3. Trenutno je mogoče konfigurirati le en pravilnik o zapadlosti za skupine v storitvi Office 365 v najemnika.
4. Skupino lahko podaljšate le globalni skrbniki, skrbniki skupine, skrbniki uporabnika in lastnik skupine.
5. Če je skupina Office 365 potekla, je izbrisana in jo je mogoče obnoviti le do 30 dni, preden pride do trajnega brisanja. Ko je skupina trajno izbrisana, je ni več mogoče obnoviti. Preberite več o obnavljanju skupin [tukaj](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Samodejna obnovitev dejavnosti**

Dejavnosti uporabnikov iz SharePointa, Outlook in Teams lahko sprožijo samodejno podaljšanje skupine. Dejavnosti so preverjene na 35 dni, preden skupina poteče. Če je na voljo aktivnost med trenutnim življenjskim ciklom skupine, bo skupina samodejno obnovljena, e-poštno obvestilo pa ne bo poslano lastnikom skupine.

**Časovna razporeditev obvestil za potekle skupine**

1. E-poštna obvestila so poslana lastnikom skupine v sistemu Office 365 30 dni, 15 dni in 1 dan pred iztekom skupine.
2. Ko prvič nastavite potek, so vse skupine, ki so starejše od intervala poteka, nastavljene na 35 dni do poteka.
3. Datum poteka skupine je izračunan na podlagi datuma podaljšanja skupine, ne glede na datum posodobljenega pravilnika. Če je pravilnik o zapadlosti posodobljen, se datum poteka ne spremeni.
4. Če želite več informacij, glejte [pravilnik o zapadlosti skupine in e-poštna sporočila](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) ter [obnovite izbrisano skupino sistema Office 365 v imeniku Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Dovoljenje za ustvarjanje skupine**

Zagotovite, da imate dovoljenje za ustvarjanje nove skupine. Globalni skrbniki lahko onemogočijo ustvarjanje skupine v portalu Azure ali v Accessovi plošči. Morda boste potrebovali skrbnika, če želite ustvariti novo skupino za vas ali pa vam dati ustrezna dovoljenja.

1. [Ustvarjanje nove skupine in dodajanje članov v portalu Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Ustvarjanje skupin v lupini PowerShell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Onemogočanje ustvarjanja skupin v lupini PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Upravljanje, kdo lahko ustvari skupine v storitvi Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Onemogočanje obvestila o storitvi Office 365 iz lupine PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Skrbniške vloge za Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Upravljanje dovoljenj za ustvarjanje skupin**

1. Globalni skrbniki lahko upravljajo dovoljenja za ustvarjanje skupine za varnostne ali Officeove skupine za 365, ki so bile ustvarjene v portalu Azure ali v Accessovi plošči, tako da **lahko uporabniki ustvarijo varnostne skupine** v storitvi Azure portali ali **Uporabniki lahko ustvarijo skupine Office 365 v nastavitvah storitve Azure portali** v **vseh skupinah > splošno (nastavitve)**.
2. Lahko tudi omejite ustvarjanje skupine, če želite izbrati skupino uporabnikov, če imate licenco Azure AD P1 Premium.

**Onemogočanje pozdravne priglasitve za nove člane skupine sistema Office 365**

Pozdravno obvestilo, poslano uporabnikom, ki so dodani v skupine sistema Office 365, lahko onemogočite tako, `UnifiedGroupWelcomeMessageEnabled` da nastavite **FALSE** v lupini PowerShell. Preberite več o tej nastavitvi [tukaj](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













