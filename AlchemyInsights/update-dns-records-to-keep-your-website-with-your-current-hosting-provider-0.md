---
title: Posodobiti zapise DNS, da vaše spletne strani s svojega trenutnega ponudnika gostovanja
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665776"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Posodobiti zapise DNS, da vaše spletne strani s svojega trenutnega ponudnika gostovanja

1. V centru Microsoft 365 admin, pojdite na **Setup** > [področja](https://portal.office.com/adminportal/home#/Domains) strani, in na seznamu domen, izberite domeno, ki jo uporabljate za vaše spletne strani.

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
