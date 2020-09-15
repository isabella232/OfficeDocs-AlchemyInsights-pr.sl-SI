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
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663529"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodajanje zunanjih uporabnikov v skupino prejemnikov

Dodajanje zunanjega stika v skupino prejemnikov (DG) je postopek v dveh korakih:
  
1. Ustvarjanje poštnega stika za zunanjega uporabnika:
    
    1. V skrbniškem središču pojdite na **Users**  >  stran[stiki](https://admin.microsoft.com/adminportal/home#/Contact) z uporabniki. 
    
    2. Izberite **Dodaj stik**.
    
    3. Vnesite podatke za stik in izberite **Dodaj**.
    
2. Dodajte poštni stik v GD:
    
    1. V skrbniškem središču pojdite na stran skupine **skupin**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Poiščite generalnega direktorata, ki ga želite dodati zunanjemu uporabniku, in ga izberite, da odprete pogovorno okno za urejanje.
    
    3. Na zavihku **člani** izberite **Ogled vseh in upravljanje članov**. 
    
    4. Izberite **Dodaj člane**.
    
    5. Izberite poštni stik, ki ste ga ustvarili v prejšnjem koraku, in nato izberite **Shrani**.
    
Če po teh navodilih zunanji uporabniki ne morejo poslati e-poštnih sporočil generalnemu direktoratu ali pa ne prejemajo e-poštnih sporočil, je to lahko, da je GD označen le za e-poštna sporočila internih uporabnikov. To konfiguracijo lahko preverite in jo odpravite tako, da upoštevate navodila [tukaj](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Opomba:** Ta navodila ne veljajo, če je vrsta skupine» skupina Microsoft 365 «namesto» skupina prejemnikov «. Če je to res, lahko zunanjega uporabnika dodate neposredno v skupino iz Outlooka. V [tem članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)so na voljo podrobne informacije o skupinah v storitvi Microsoft 365, kot tudi navodila za dodajanje zunanjih gostov.
  