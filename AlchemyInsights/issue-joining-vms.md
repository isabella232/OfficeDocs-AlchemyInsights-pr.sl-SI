---
title: Težave s pridružitvijo VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885661"
---
# <a name="issue-joining-vms"></a>Težave s pridružitvijo VMs

Če želite odpraviti težave, ki se pojavijo med poskusom združevanja VMs, izvedite te korake:

1. Poskusite se vpisati z obliko **UPN** (na primer» joeuser@contoso.com «), namesto v obliki zapisa **SAMAccountName** (» CONTOSO\joeuser «).
2. Zagotovite, da ste omogočili sinhronizacijo gesel v skladu z navodili, opisanimi v vodniku *za uvod.*
3. Zagotovite, da prizadeti uporabniški račun ni zunanji račun v storitvi Azure AD najemnik. Zunanji uporabniki se ne morejo vpisati v upravljano domeno, saj storitve Azure AD Domain Services nimajo poverilnic za te uporabniške račune.
4. Če je prizadeti uporabniški račun le uporabniški račun v oblaku, zagotovite, da so uporabniki spremenili svoje geslo, potem ko ste omogočili domenske storitve Azure AD. Ta korak povzroči, da so vrednosti za poverilnice, ki jih potrebujete za storitev Azure AD Domain, ustvarjene.
5. Če so prizadeti uporabniški računi sinhronizirani iz imenika na mestu uporabe, preverite, ali je bila priporočena izdaja storitve Azure AD Connect konfigurirana tako, da izvaja popolno sinhronizacijo.
6. Če težave ne morete odpraviti po potrditvi koraka 4, izvedite te ukaze iz sinhronizacijskega računalnika:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.