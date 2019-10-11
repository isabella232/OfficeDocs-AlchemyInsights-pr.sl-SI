---
title: Zaljubljen v odpošiljanju zaradi velikih prilog
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441321"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Popravljanje sporočil, ki so obtičala v mapi» Odpošlji «

Priporočamo, da začnete tako, da zaženete scenarij [» Imam težave pri pošiljanju, prejemanju ali iskanju e-poštnih sporočil «](https://aka.ms/SaRA-OutlookSendReceive) iz [Microsoftovega orodja za podporo in obnovitev](https://diagnostics.office.com/#/) .

Ko se sporočilo v mapi» Odpošlji «ujame, so najverjetnejši vzroki:
- Velike priponke.
- **Pošlji takoj, ko je povezana** možnost ni omogočena.

Če želite odstraniti velike Priloge: 

1. V Outlooku izberite **Pošlji/Prejmi** > **delo brez povezave**. 
2. V podoknu za krmarjenje izberite **Odpošlji**. Od tu lahko: 
    - Izbrišite sporočilo (izberite ga in izberite **Izbriši**).
    - Povlecite sporočilo v mapo Osnutki, dvokliknite, da ga odprete, in odstranite Prilogo in izberite **Izbriši**).
3. Če se prikaže napaka, ki pravi, da Outlook poskuša posredovati sporočilo, zaprite Outlook. Lahko traja nekaj trenutkov za izhod. Če se Outlook ne zapre, pritisnite CTRL + ALT + DELETE in izberite **Zaženi upravitelja opravil**. V upravitelju opravil izberite zavihek **procesi** , se pomaknite navzdol do možnosti Outlook. exe in izberite **Končaj proces**.
4. Ko se Outlook zapre, ga znova zaženite in ponovite korake 2 in 3. 
5. Ko odstranite Prilogo, kliknite **Pošlji/Prejmi** > **delo brez povezave** , da nadaljujete delo v spletu. 

Sporočila se tudi zataknejo v mapi» **Odpošlji**«, ko kliknete Pošlji, vendar niste povezani. Kliknite **Pošlji/Prejmi** in si oglejte **delovni gumb brez povezave** . Če je modra, si izključen. Izberite jo za povezavo (gumb se obarva belo) in kliknite **Pošlji vse**.
 
Če želite omogočiti **pošiljanje takoj, ko je priključen**:
 
- Izberite **** > **** možnosti >  datoteke**Napredno**.
V odseku **Pošlji in prejmi** izberite **Pošlji takoj, ko je povezava vzpostavljena**, nato pa izberite **v redu**.
 
Za podrobnejše informacije glej:
- [Videoposnetek: pošiljanje ali brisanje zagozdila e-poštnega sporočila](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-pošta ostane v mapi» Odpošlji «, dokler ročno ne sprožite operacije pošiljanja/prejemanja v programu Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
