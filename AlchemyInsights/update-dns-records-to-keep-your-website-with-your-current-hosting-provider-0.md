---
title: Posodabljanje zapisov DNS za obdržite spletno mesto pri trenutnem ponudniku gostovanja
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007698"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Posodabljanje zapisov DNS za obdržite spletno mesto pri trenutnem ponudniku gostovanja

1. V Skrbniško središče za Microsoft 365 izberite stran **Setup** Domains (Nastavitve domen) in na seznamu domen izberite domeno, ki jo uporabljate  >  [](https://admin.microsoft.com/Adminportal#/Domains) za svoje spletno mesto.

2. Izberite **+ Nov zapis po** meri in vnesite to:

  - Za **vrsto DNS** vnesite: A **(naslov)**

  - Za **Ime ali vzdevek gostitelja** vnesite to: **@**

  - Za **Naslov IP** vnesite statičen naslov IP za spletno mesto, kjer trenutno gostuje (na primer, 172.16.140.1).

    To mora biti  *statični*  naslov IP za spletno mesto in ne  *dinamičen*  naslov IP. Preverite, kje gostuje vaše spletno mesto, da boste lahko dobili statičen naslov IP za svoje javno spletno mesto.

3. Izberite **Shrani**.

Poleg tega lahko ustvarite zapis CNAME, da bodo stranke lahko pomagale najti vaše spletno mesto.
  
1. Izberite **+ Nov zapis po** meri in vnesite to:

  - Za **vrsto DNS** vnesite: **CNAME (vzdevek)**

  - Za **Ime ali vzdevek gostitelja** vnesite to: **www**

  - V **polje Kaže na** naslov vnesite popolnoma določeno ime domene (FQDN) za spletno mesto (na primer contoso.com).

2. Izberite **Shrani**.
