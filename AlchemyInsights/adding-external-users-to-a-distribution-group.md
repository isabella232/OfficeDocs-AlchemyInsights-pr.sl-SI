---
title: Dodajanje zunanjih uporabnikov v distribucijsko skupino
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737889"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodajanje zunanjih uporabnikov v distribucijsko skupino

Dodajanje zunanjega stika distribucijski skupini (DG) je postopek v dveh korakih:
  
1. Ustvarite e-poštni stik za zunanjega uporabnika:
    
    1. V skrbniškem središču pojdite na stran» **** > [stiki](https://admin.microsoft.com/adminportal/home#/Contact) uporabnikov «. 
    
    2. Izberite **Dodaj vizitko**.
    
    3. Vnesite informacije za stik in izberite **Dodaj**.
    
2. Dodajanje e-poštnega stika v svoj GD:
    
    1. V skrbniškem središču pojdite[na stran](https://admin.microsoft.com/adminportal/home#/groups) skupine **skupin** > . 
    
    2. Poiščite GD, ki ga želite dodati zunanjemu uporabniku, in ga izberite, da odprete pogovorno okno za urejanje.
    
    3. Na zavihku» **člani** «izberite **Prikaži vse in upravljajte člane**. 
    
    4. Izberite **Dodaj člane**.
    
    5. Izberite e-poštni stik, ki ste ga ustvarili v prejšnjem koraku, in nato izberite **Shrani**.
    
Če po tem postopku zunanji uporabniki ne morejo pošiljati e-poštnih sporočil generalnemu direktoratu ali ne prejemajo e-poštnih sporočil, je lahko to, da je GD označen samo za omogočanje e-poštnih sporočil od notranjih uporabnikov. To konfiguracijo lahko preverite in odpravite po navodilih [tukaj](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Opomba:** Ta navodila ne veljajo, če je vrsta skupine» skupina Office 365 «namesto» skupina prejemnikov «. V tem primeru lahko zunanjega uporabnika dodate neposredno v skupino iz Outlooka. Podrobne informacije o skupini Office 365 in navodila za dodajanje zunanjih gostov so na voljo v [tem članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  