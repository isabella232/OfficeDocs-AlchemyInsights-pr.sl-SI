---
title: Dodajanje zunanjih uporabnikov v skupino prejemnikov
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934849"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodajanje zunanjih uporabnikov v skupino prejemnikov

Dodajanje zunanjega stika v skupino prejemnikov je postopek v dveh korakih:
  
1. Ustvarjanje poštnega stika za zunanjega uporabnika:
    
    1. V skrbniškem središču odprite stran **Stiki**  >  [](https://admin.microsoft.com/adminportal/home#/Contact) uporabnikov. 
    
    2. Izberite **Dodaj stik.**
    
    3. Vnesite informacije za stik in izberite **Dodaj**.
    
2. Dodajanje poštnega stika v skupino za skupino stikov:
    
    1. V skrbniškem središču pojdite na **stran**  >  [Skupine](https://admin.microsoft.com/adminportal/home#/groups) skupin. 
    
    2. Poiščite skupine skupine uporabnikov, v katerega želite dodati zunanjega uporabnika, in jo izberite, da odprete pogovorno okno za urejanje.
    
    3. Na **zavihku** Člani izberite Ogled **vseh in upravljanje članov.** 
    
    4. Izberite **Dodaj člane.**
    
    5. Izberite poštni stik, ki ste ga ustvarili v prejšnjem koraku, nato pa izberite **Shrani**.
    
Če zunanji uporabniki po tem postopku ne morejo pošiljati e-poštnih sporočil skupine uporabnikov ali od njih prejemati e-poštnih sporočil, je morda skupine skupine uporabnikov označena tako, da dovoli le e-pošto notranjih uporabnikov. To konfiguracijo lahko preverite in jo popravite tako, da sledite navodilom [tukaj.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Opomba:** Ta navodila ne veljajo, če je vrsta vaše skupine »Microsoft 365« in ne »skupina prejemnikov«. V tem primeru lahko dodate zunanjega uporabnika neposredno v skupino iz Outlook. Podrobne informacije o gostje Microsoft 365 skupine in navodila za dodajanje zunanjih gostov so na voljo v tem [članku.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  