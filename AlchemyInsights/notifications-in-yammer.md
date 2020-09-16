---
title: Obvestila v aplikaciji Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: c1fbeea7bf4269e90e52cf5c129e904c99714926
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662809"
---
# <a name="notifications-in-yammer"></a>Obvestila v aplikaciji Yammer

Ker vas želimo opozoriti na novo dejavnost v ustreznih pogovorih, [aplikacija Yammer pošilja obvestila](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) prek e-pošte, če pa uporabljate aplikacijo Yammer v prenosni napravi, prek potisnih obvestil. Aplikacija Yammer pošilja obvestila za številne vrste dejavnosti v vašem omrežju. Uporabniki lahko svoje nastavitve e-pošte posodobijo na spletnem mestu aplikacije Yammer, potisna obvestila pa so konfigurirana prek mobilne aplikacije. 

Z aplikacijo Yammer je bila dodana podpora za [interaktivna e-poštna sporočila v Outlooku](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Nekatera e-poštna sporočila (kopijo sporočila) bodo postala interaktivna v Outlooku v spletu. S prihodnjo posodobitvijo bo ta funkcija na voljo v drugih različicah Outlooka.

**Vrste obvestil v aplikaciji Yammer**

- E-poštna sporočila (Posodobitve iz skupine, nekdo vas povabi v skupino, prejmete sporočilo v mapo »Prejeto« itd.)
- Potisna obvestila (Poslano v prenosne naprave, ko vas nekdo omeni, prejmete sporočilo v mapo »Prejeto« itd.)
- Pojavna obvestila na namizju (Ko imate nameščeno namizno različico aplikacije Yammer, prikaže obvestila za uporabnike.)
- Obvestila z zvoncem (Na spletnem mestu aplikacije Yammer bodo uporabniki videli obvestila za različne dogodke. Ni nujno, da bo s temi obvestili vedno povezano e-poštno ali potisno obvestilo.)

Na voljo je več [podrobnih informacij o obvestilih](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Upravljanje obvestil**

Uporabniki morajo upravljati svoja lastna obvestila. Na voljo so informacije o tem, [kako omogočite in onemogočite e-poštna obvestila in obvestila v prenosnih napravah aplikacije Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Skrbniki ne morejo onemogočiti vsa obvestila ali nadzorovati obvestil v imenu uporabnikov. Skrbniki lahko [nadzorujejo logotip, vključen v e-poštna sporočila, in ali morajo uporabniki potrditi sporočila,](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) poslana z e-pošto.

**E-poštna obvestila, poslana številnim uporabnikom v organizaciji**

Včasih bo aplikacija Yammer poslala eno e-poštno obvestilo, ki ga bo prejelo precej večje število uporabnikov v organizaciji od pričakovanega. Do tega pride takrat, ko je v aplikacijo Yammer dodan seznam prejemnikov ali druga vrsta e-poštnega naslova, ki se ne nanaša na posameznika. Aplikacija Yammer ne ve vedno, ali e-poštni naslov pripada posameznemu uporabniku ali pa gre za e-poštni naslov, s katerim bo eno e-poštno sporočilo dostavljeno številnim prejemnikom. Ko pride do te težave, morate ukrepati in aplikaciji Yammer [začasno ustaviti (deaktivirati) neveljavnega uporabnika s tem e-poštnim naslovom](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users). 

Če želite zmanjšati možnost, da pride do te težave:

1. [Vsilite identiteto storitve Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) za Yammer.
2. Onemogočite zunanjim pošiljateljem pošiljanje e-pošte v organizacijo ali omejite število pošiljateljev na seznam odobrenih.

Če pride do te težave:

1. Identificirajte prejemnika e-pošte, ki bi se moral ujemati z uporabnikom v aplikaciji Yammer. Na primer vsi-v-prodaji@fabrikam.com je seznam prejemnikov za vse prodajalce. Seznam prejemnikov bi bilo mogoče prepoznati na podlagi e-pošte aplikacije Yammer, ki bi jo prejeli uporabniki.
2. Uporabite [funkcijo za deaktiviranje (začasno onemogočenje) v razdelku skrbnika omrežja](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) in začasno onemogočite uporabnika z e-poštnim naslovom vsi-v-prodaji@fabrikam.com. Začasno onemogočenje je mogoče razveljaviti, zato je to bolj varno kot izbris. Uporabnik bo samodejno izbrisan po 90 dneh.
3. Lahko tudi pregledate [izvoz uporabnika](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers), da identificirate druge e-poštne naslove, ki se ne nanašajo na posameznika, ki bi jih bilo treba začasno onemogočiti.
