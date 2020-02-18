---
title: Pravilnika» Allowselfservicenabava «ni mogoče nastaviti ali si ogledati
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091766"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Pravilnika» Allowselfservicenabava «ni mogoče nastaviti ali si ogledati

Ko poskušate nastaviti ali si ogledati pravilnik Allowselfservicenabava, se prikaže to sporočilo o napaki:

*HandleError: ne zadostovati v rešitev zmnožek zvitost s PolicyId ' Allowselfservicenabava ', ErrorMessage-osnovna povezava je bila zaprta: Prišlo je do nepričakovane napake pri pošiljanju.*

To je lahko posledica starejše različice varnosti transportnega sloja (TLS). Če želite povezati storitev MSCommerce, morate uporabiti TLS 1,2 ali več.  

Če želite omogočiti/nastaviti protokol TLS na 1,2, preverite in poskusite znova, poskusite naslednje korake.
 1. V ukazni poziv PowerShell (PS C:\) vnesite naslednji ukaz, da NASTAVITE protokol TLS na različico 1,2:

    \[Net. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12

2. Preverite protokole TLS, ki jih uporabljate, z naslednjim ukazom:

    \[Net. ServicePointManager]:: SecurityProtocol 

3. Po potrebi znova poskusite ukaze Get ali Update.

