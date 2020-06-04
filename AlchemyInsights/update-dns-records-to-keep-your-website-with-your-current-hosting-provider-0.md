---
title: Posodobite zapise DNS, da bo vaše spletno mesto s trenutnim ponudnikom gostovanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665776"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Posodobite zapise DNS, da bo vaše spletno mesto s trenutnim ponudnikom gostovanja

1. V skrbniškem središču Microsoft 365 pojdite na stran z **nastavitvami**  >  [domen](https://portal.office.com/adminportal/home#/Domains) in na seznamu domen izberite domeno, ki jo uporabljate za spletno mesto.

2. Izberite **+ nov zapis po meri** in vnesite naslednje:

  - Za **vrsto DNS** vnesite: **A (naslov)**

  - Za **ime gostitelja ali vzdevek**vnesite to:**@**

  - Za naslov **IP**vnesite statični naslov IP za spletno mesto, kjer je trenutno gostujoča (na primer 172.16.140.1).

    To mora biti *statični* naslov IP za spletno stran, ne *dinamični* IP naslov. Preverite s strani, kjer je vaša spletna stran gostuje, da se prepričajte, da lahko dobite statični naslov IP za vašo javno spletno stran.

3. Izberite **Shrani**.

Poleg tega lahko ustvarite zapis CNAME, ki bo strankam pomagal najti vaše spletno mesto.
  
1. Izberite **+ nov zapis po meri** in vnesite naslednje:

  - Za **tip DNS** vnesite: **CNAME (alias)**

  - Za **ime gostitelja ali vzdevek**vnesite to: **www**

  - Za **točke za naslov**vnesite popolnoma kvalificirano ime domene (FQDN) za vaše spletno mesto (na primer contoso.com).

2. Izberite **Shrani**.
