---
title: Posodobiti zapise DNS, da vaše spletne strani s svojega trenutnega ponudnika gostovanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
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
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506423"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Posodobiti zapise DNS, da vaše spletne strani s svojega trenutnega ponudnika gostovanja

1. Na [področje](https://portal.office.com/adminportal/home#/Domains) strani, domen, na seznamu izberite domeno uporabljate za vašo spletno stran.

2. **+ Nov zapis po meri** in vnesite naslednje:

  - Za **DNS vrsta** vnesite: **(naslov)**

  - **Ime gostitelja ali Alias**, vnesite naslednje:**@**

  - Za **IP naslov**, vnesite statični naslov IP za vašo spletno stran, kjer je trenutno gosti (npr. 172.16.140.1).

    To mora biti *statični* naslov IP za spletno stran, ne *dinamični* IP naslov. Preveriti s mesto, kjer vašo spletno stran gostuje prepričati se lahko dobite statični naslov IP za javne spletne strani.

3. Izberite **Shrani**.

Poleg tega lahko ustvarite zapis CNAME za pomoč uporabniki našli vašo spletno stran.
  
1. **+ Nov zapis po meri** in vnesite naslednje:

  - Za **DNS vrsta** vnesite: **CNAME (Alias)**

  - **Ime gostitelja ali Alias**, vnesite naslednje: **www**

  - Za **točki naslov**, vnesite ime domene (FQDN) za vašo spletno stran (na primer contoso.com).

2. Izberite **Shrani**.
