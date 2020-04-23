---
title: Odpravljanje težav pri sinhronizaciji gesel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732526"
---
# <a name="troubleshoot-password-synchronization"></a>Odpravljanje težav pri sinhronizaciji gesel

Če želite odpraviti težave, pri katerih se gesla ne sinhronizirajo s storitvijo Azure AD Connect 1.1.614.0 ali novejšo različico:
  
1. Odprite novo sejo lupine Windows PowerShell v strežniku Azure AD Connect z možnostjo **Zaženi kot skrbnik** .

2. Zaženi **nastavljeno-ExecutionPolicy Remotepodpisano** ali **nastavljeno-ExecutionPolicy neomejen**.

3. Zaženite čarovnika za povezavo Azure AD Connect.

4. Pomaknite se na stran **dodatna opravila** , izberite **Odpravljanje težav**in kliknite **naprej**.

5. Na strani za odpravljanje težav kliknite **Zaženi, da zaženete meni za odpravljanje težav** v PowerShell.

6. V glavnem meniju izberite **Odpravljanje težav s sinhronizacijo gesel**.

7. V podmeniju izberite **sinhronizacija gesel sploh ne deluje**.

**Razumevanje rezultatov opravila za odpravljanje težav**
  
Opravilo za odpravljanje težav izvede te preglede:
  
- Potrdi, da je funkcija sinhronizacije gesel omogočena za najemnika Azure AD.

- Potrdi, da strežnik Azure AD Connect ni v načinu Stopnjevitost.

- Za vsak obstoječi krajevni konektor imenika Active Directory (ki ustreza obstoječemu gozdu imenika Active Directory):

- 
  - Potrdi, da je funkcija sinhronizacije gesel omogočena.

  - Poišče dogodke srčnega utripa za sinhronizacijo gesel v dnevnikih programa Windows Application Event.

  - Za vsako domeno imenika Active Directory pod krajevnim konektorjem imenika Active Directory:

  - Preveri, ali je domena dosegljiva iz strežnika Azure AD Connect.

  - Preveri, ali so računi storitve Active Directory (AD DS), ki jih uporablja krajevni konektor imenika Active Directory, pravilno uporabniško ime, geslo in dovoljenja, potrebna za sinhronizacijo gesel.

Če želite več pomoči pri sinhronizaciji gesel, glejte [Odpravljanje težav s sinhronizacijo gesel s sinhronizacijo AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  