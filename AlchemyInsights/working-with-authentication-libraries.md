---
title: Delo s knjižnicami za preverjanje pristnosti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036868"
---
# <a name="working-with-authentication-libraries"></a>Delo s knjižnicami za preverjanje pristnosti

Če želite odpraviti težavo z Microsoftovo knjižnico za preverjanje pristnosti (MSAL), izvedite te priporočene korake:

1. **Delo z MSAL**: [knjižnice za preverjanje pristnosti za Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – v tem članku je prikazana podpora knjižnice za Microsoft preverjanje pristnosti za več vrst aplikacij. Vključuje povezave do izvorne kode knjižnice; kje dobiti paket za projekt programa; in ali knjižnica podpira vpis uporabnika (preverjanje pristnosti), dostop do zaščitenih spletnih vmesnikov API (avtorizacija) ali oboje.

2. **Odpravljanje težav s preverjanjem pristnosti**: MSAL podpira več tokov preverjanja pristnosti za uporabo v različnih scenarijih programov. Odvisno od tega, kako je vaš odjemalski program zgrajen, lahko MSAL uporabi enega ali več tokov preverjanja pristnosti, ki jih podpira Microsoftova platforma Identity. Ti tokovi lahko ustvarijo več vrst žetonov in šifer dovoljenj ter zahtevajo različne žetone, da bodo delovali.

3. **Žetoni za dostop**: [žetoni za dostop do Microsoftovega](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) uporabniškega vmesnika – Preberite, kako lahko API preveri veljavnost in uporabi terjatve znotraj žetona za dostop. Vsa dokumentacija v tem članku, razen če je označeno, velja le za žetone, izdane za API-je, ki ste jih registrirali. Ne velja za žetone, izdane za Microsoft lastne API-je, ne morete pa uporabiti teh žetonov za preverjanje, kako Microsoftova identitetna platforma izdaja žetone za API, ki jih ustvarite.

**Konec podpore za knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice ADAL)**

- Z **začetkom junija 30th 2020** ne bomo več dodali nobenih novih funkcij v knjižnice adal in Azure ad Graph. Še naprej nudimo tehnično podporo in varnostne posodobitve, ne zagotavljamo pa več posodobitev funkcij.
- Z **začetkom junija 30th 2022** bomo zaključili podporo za knjižnice adal in Azure ad Graph in ne boste več zagotavljali tehnične podpore ali varnostnih posodobitev.
- Programi, ki uporabljajo knjižnice ADAL v obstoječih različicah sistema OS, bodo po tem času še naprej delovali, vendar ne bodo *prejeli nobene tehnične podpore ali varnostnih posodobitev*.
- Programi, ki uporabljajo Azure AD Graph, po tem času morda ne bodo več prejemali odgovorov iz končne točke grafikona Azure AD.

**Selitev v knjižnice ADAL**

- Priporočamo, da posodobite MSAL, ki vsebuje najnovejše funkcije in varnostne posodobitve.
- Če uporabljate Microsoft apps, morate vedeti, da je Microsoft v postopku selitve svojih programov v MSAL s končnim rokom za konec podpore, ki zagotavlja, da bodo imeli koristi od trenutne varnosti in izboljšav funkcij v MSAL.

1. [Preberite pogosta vprašanja o knjižnice adal](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Preberite več o tem, kako preseliti aplikacije na osnovi na platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Če imate po branju priročnika za platformo aplikacije na voljo dodatna vprašanja, lahko objavite na [spletnem mestu Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) z oznako [Azure-ad-knjižnice adal-zastaranje] ali pa odprete težavo v skladišču mesta GitHub v knjižnici. Oglejte si razdelek [jeziki in okviri](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) v članku **MSAL pregled** članka za povezave do repo posameznih knjižnic.
4. **Če potrebujete pomoč pri razumevanju, kateri programi uporabljajo knjižnice adal**, priporočamo, da pregledate vse izvorne kode aplikacije. Po potrebi se povežite s katerim koli neodvisnim prodajalcem programske opreme (ISVs) ali ponudnikom aplikacij. Microsoftova podpora vam lahko posreduje seznam vseh aplikacij ADAL v vašem najemniku, ki jih ne zagotavlja Microsoft.







