---
title: Dodajanje zunanjih uporabnikov v distribucijsko skupino
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910948"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodajanje zunanjih uporabnikov v distribucijsko skupino

Dodajanje zunanjega stika distribucijski skupini (DG) je postopek v dveh korakih:
  
1. Ustvarite e-poštni stik za zunanjega uporabnika:
    
    1. V skrbniškem središču pojdite na stran» **Users** > [stiki](https://admin.microsoft.com/adminportal/home#/Contact) uporabnikov «. 
    
    2. Izberite **Dodaj vizitko**.
    
    3. Vnesite informacije za stik in izberite **Dodaj**.
    
2. Dodajanje e-poštnega stika v svoj GD:
    
    1. V skrbniškem središču pojdite[na stran](https://admin.microsoft.com/adminportal/home#/groups) skupine **skupin** > . 
    
    2. Poiščite GD, ki ga želite dodati zunanjemu uporabniku, in ga izberite, da odprete pogovorno okno za urejanje.
    
    3. Na zavihku» **člani** «izberite **Prikaži vse in upravljajte člane**. 
    
    4. Izberite **Dodaj člane**.
    
    5. Izberite e-poštni stik, ki ste ga ustvarili v prejšnjem koraku, in nato izberite **Shrani**.
    
Če po tem postopku zunanji uporabniki ne morejo pošiljati e-poštnih sporočil generalnemu direktoratu ali ne prejemajo e-poštnih sporočil, je lahko to, da je GD označen samo za omogočanje e-poštnih sporočil od notranjih uporabnikov. To konfiguracijo lahko preverite in odpravite po navodilih [tukaj](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Opomba:** Ta navodila ne veljajo, če je vrsta skupine» skupina Microsoft 365 «namesto» skupina prejemnikov «. V tem primeru lahko zunanjega uporabnika dodate neposredno v skupino iz Outlooka. Podrobne informacije o Microsoftovih 365 skupinah gostov, kot tudi navodila za dodajanje zunanjih gostov, je mogoče najti v [tem članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  