---
title: Posodobitev zapisov DNS za ohranjanje spletnega mesta s trenutnim ponudnikom gostovanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815801"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Posodobitev zapisov DNS za ohranjanje spletnega mesta s trenutnim ponudnikom gostovanja

1. V skrbniškem središču za Microsoft 365 pojdite na stran **Nastavitev**  >  [domen](https://admin.microsoft.com/Adminportal#/Domains) in na seznamu domen izberite domeno, ki jo uporabljate za spletno mesto.

2. Izberite **+ nov zapis po meri** in vnesite to:

  - Za **vrsto DNS** vnesite: **A (naslov)**

  - Za **ime ali vzdevek gostitelja**vnesite to: **@**

  - Za **naslov IP**vnesite statični naslov IP za spletno mesto, kjer trenutno gostuje (na primer: 172.16.140.1).

    To mora biti  *statični*  naslov IP za spletno mesto, ne pa  *dinamični*  naslov IP. Obiščite spletno mesto, kjer gostuje spletno mesto, da se prepričate, da lahko dobite statični naslov IP za javno spletno mesto.

3. Izberite **Shrani**.

Poleg tega lahko ustvarite zapis CNAME za pomoč uporabnikom pri iskanju spletnega mesta.
  
1. Izberite **+ nov zapis po meri** in vnesite to:

  - Za **vrsto DNS** vnesite: **CNAME (vzdevek)**

  - Za **ime ali vzdevek gostitelja**vnesite to: **www**

  - Za **točke na naslov**vnesite popolnoma določeno ime domene (FQDN) za vaše spletno mesto (na primer contoso.com).

2. Izberite **Shrani**.
