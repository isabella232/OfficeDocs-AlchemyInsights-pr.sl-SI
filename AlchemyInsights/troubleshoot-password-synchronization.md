---
title: Odpravljanje težav s sinhronizacijo geslo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 589820c945fb20f00431655f9f53196e740bb38f
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655827"
---
# <a name="troubleshoot-password-synchronization"></a>Odpravljanje težav s sinhronizacijo geslo

Za odpravljanje težav, kjer brez gesla so sinhronizirani z Azure AD povezavo različico 1.1.614.0 ali novejšo različico:
  
1. Odprite novo sejo lupine Windows PowerShell na strežniku Azure AD povezavo s **prost dostop kot oskrbnik** predkupna pravica. 
    
2. Teči **niz-pravilnika o izvajanju lupine RemoteSigned** ali **niz-pravilnika o izvajanju lupine neomejen**. 
    
3. Zagnati čarovnika Azure AD povezavo.
    
4. Pluti v ** dodatne naloge ** strani, izberite ** odpravljanje **, in kliknite **naprej**. 
    
5. Na strani odpravljanje težav, kliknite meni **začetek za začetek odpravljanja napak** v lupini PowerShell. 
    
6. V glavnem meniju, izberite **Odpravljanje težav s sinhronizacijo geslo**. 
    
7. V podmeniju, izberite **sinhronizacijo geslo ne dela na vseh**. 
    
 **Spoznajo rezultate opravila, odpravljanje težav**
  
Odpravljanje težav nalogo opravlja naslednje preglede:
  
- Potrjuje, da je geslo sinhronizacijo možnost omogočena za modro AD najemnik.
    
- Potrjuje, da Azure AD Connect strežnikom ni v produkcijskem načinu.
    
- Za vsak obstoječi krajevni Active Directory priključek (kar ustreza obstoječemu gozdu Active Directory):
    
- 
  - Potrjuje, da je omogočena funkcija za sinhronizacijo geslo.
    
  - Išče geslo sinhronizacijo srčni utrip dogodkov v dnevnikih dogodkov za program Windows.
    
  - Za vsako domeno Active Directory pod priključek krajevnega imenika Active Directory:
    
  - Potrjuje, da je dosegljiv iz Azure AD povezavo strežnika domene.
    
  - Potrjuje, da domene storitve Active Directory (AD DS) kontov, s krajevnim Active Directory priključek je pravilno uporabniško ime, geslo in dovoljenja, zahtevana za sinhronizacijo geslo.
    
Pomoč parola omedlevičen za odpravljanje težav, glejte [Odpravljanje geslo sinhronizacije z Azure AD povezavo sinhronizacijo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

