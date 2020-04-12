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
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232646"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Popravljanje sporočil, ki so obtičala v mapi» Odpošlji «

Priporočamo, da začnete tako, da zaženete scenarij [» Imam težave pri pošiljanju, prejemanju ali iskanju e-poštnih sporočil «](https://aka.ms/SaRA-OutlookSendReceive) iz [Microsoftovega orodja za podporo in obnovitev](https://diagnostics.office.com/#/) v prizadetem računalniku.

Ko se sporočilo zatakne v mapi» Odpošlji «, je najverjetnejši vzrok velika pripona ali možnost» Pošlji takoj, ko je vzpostavljena povezava «ni omogočena.

**Odstranjevanje velike pritrditve**

1. Kliknite **Pošlji/Prejmi** > **delo brez povezave**. 
2. V podoknu za krmarjenje kliknite **Odpošlji**. Od tu lahko: 
    - Izbrišite sporočilo. Šele izbrati to ter udarjanje z nogo ob nogo **izbrisati**.
    - Povlecite sporočilo v **mapo Osnutki**, dvokliknite, da odprete sporočilo, in izbrišite Prilogo (kliknite nanj in kliknite **Izbriši**).
3. Če napaka pove, da Outlook poskuša posredovati sporočilo, zaprite Outlook. Lahko traja nekaj trenutkov za izhod. Če se Outlook ne zapre, pritisnite **CTRL + ALT + DELETE** in kliknite **Zaženi upravitelja opravil**. V upravitelju opravil izberite zavihek **procesi** , se pomaknite navzdol do možnosti Outlook. exe in kliknite **Končaj proces**.
4. Ko se Outlook zapre, znova zaženite Outlook in ponovite korake 2-3. 
5. Ko odstranite Prilogo, kliknite **Pošlji/Prejmi** > **delo brez povezave** , da počistite gumb in nadaljujete delo v spletu. 

Sporočila se tudi zataknejo v mapi» **Odpošlji**«, ko kliknete Pošlji, vendar niste povezani. Kliknite **Pošlji/Prejmi** in si oglejte **delovni gumb brez povezave** . Če je modra, si izključen. Kliknite na povezavo (gumb se obarva belo) in kliknite **Pošlji vse**.
 
**Omogoči pošiljanje takoj, ko je priključen**
 
1. Na kartici Datoteka kliknite **možnosti**.

2. V pogovornem oknu možnosti programa Outlook kliknite **Napredno**.

3. V odseku Pošlji in prejmi kliknite, če želite omogočiti **pošiljanje takoj, ko je priključen**. Kliknite **V redu**.
 
Za vse podrobnosti glejte:
- [Videoposnetek: pošiljanje ali brisanje zagozdila e-poštnega sporočila](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-pošta ostane v mapi» Odpošlji «, dokler ročno ne sprožite operacije pošiljanja/prejemanja v programu Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
