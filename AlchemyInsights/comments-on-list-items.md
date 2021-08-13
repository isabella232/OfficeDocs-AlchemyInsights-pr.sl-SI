---
title: Pripombe o elementih seznama
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995505"
---
# <a name="comments-on-list-items"></a>Pripombe o elementih seznama

Uporabniki si lahko ogledajo vse pripombe elementa seznama in filtrirajo med pogledi, ki prikazujejo pripombe ali dejavnosti, povezane z elementom.

Preden lahko uporabniki dodajajo in brišejo pripombe, morajo zabeležiti to:

- Pripombe sledijo nastavitvam dovoljenj, ki so v SharePoint.
- Klasični seznami, ki še niso vgrajeni za prikaz v sodobnih uporabniških vmesnikih, kot so seznami opravil, ne bodo imeli te funkcije za komentiranje.
- Komentiranje seznamov v Teams ni na voljo v tej izdaji.
- Iskanje ne indeksira pripomb.

Skrbniki lahko onemogočijo to funkcijo na ravni organizacije tako, da spreminjajo parameter **CommentsOnListItemsDisabled** v ukazu »cmdlet« **Set-SPOTenant** PowerShell.

Trenutno ni mogoče onemogočiti komentiranja na ravni mesta ali seznama. Upamo, da bodo ti kontrolniki na voljo v poznejši posodobitvi, verjetno v prvem četrtletju leta 2021.
