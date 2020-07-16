---
title: Izdaja odpiranja ali prenosa datotek v storitvi Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148341"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Izdaja odpiranja ali prenosa datotek v storitvi Yammer

Classic Yammer podpira več možnosti za nalaganje datotek v sporočila in skupine. Glede na konfiguracijo omrežja so datoteke privzete za shranjevanje v SharePointu.

Izbirnik datotek v novi storitvi Yammer še ne podpira vseh možnosti, ki so na voljo v klasični storitvi Yammer. Prihodnja posodobitev bo dodala dodatne funkcije. Če želite več informacij, glejte [prilaganje datoteke ali slike v mesto pogovora v storitvi Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Datoteke ni mogoče odpreti ali prenesti**  

Datoteka se lahko naloži v storitev Yammer, vendar se poveže tudi z datoteko v storitvi SharePoint online. Če želite odpraviti težave, morate najprej določiti lokacijo datoteke. Če je bila datoteka naložena v storitev Yammer, bo imela URL *. yammer.com. Zagotovite, da so zahtevani URL-ji in naslovi IP neblokirani. Če želite več informacij, glejte objavo v spletnem dnevniku [z uporabo trdih kodiranih IP naslovov za Yammer ni priporočljiva](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Preverite, ali lahko uporabnik, ki je tudi globalni skrbnik, prenese datoteko. Če je datoteka zasebna, boste morda morali uporabiti način zasebnega vsebine. Če želite več informacij, glejte [spremljanje zasebne vsebine v storitvi Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Gosti in datoteke na ravni omrežja yammer v storitvi SharePoint online**  

[Gosti na ravni omrežja v storitvi Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ne uporabljajo storitve AZURE ad B2B in so notranji v storitvi yammer, zato ne morejo dostopati do datotek yammer, shranjenih v SharePointu. Ustvarite zunanjega uporabnika AAD B2B, ki lahko dostopa do knjižnic dokumentov v SharePoint online z uporabo te identitete. Če želite več informacij o prihodnji podpori za gostjo Azure AD B2B v storitvi Yammer, si oglejte [podporo za podjetja v storitvi Yammer preview – pogoji za stranke in pogosta vprašanja](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).