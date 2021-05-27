---
title: Pri odpravljanju težav z e-odkrivanjem pride do napak
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676283"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Pri odpravljanju težav z e-odkrivanjem pride do napak

Ali imate težave z zadržanjem e-odkrivanja? Tukaj je nekaj najboljših praks, na voljo:

- Preverite stanje zadržanja porazdelitve.  Če je stanje **»Izklopljeno« (v čakanju)** ali **»Izklopljeno« (v čakanju),** počakajte, da se porazdelitev konča.
- Spojite posodobitve zadržanja e-odkrivanja v eno množično zahtevo, namesto da bi večkrat posodobili pravilnik za vsako transakcijo.
- Zaženite Set-CaseHoldPolicy <policyname> -RetryDistribution v Powershell središču za varnost in skladnost s predpisi. Podrobnosti najdete v Povezovalnik [PowerShell v središču za & in skladnost s predpisi.](/powershell/exchange/connect-to-scc-powershell)

Če želite navodila za preverjanje teh nastavitev in dodatnih najboljših praks za omiljenje in odpravljanje težav z e-odkrivanjem, glejte Odpravljanje napak zadržanja [e-odkrivanja.](/microsoft-365/compliance/hold-distribution-errors)
Če želite več informacij o odpravljanju drugih pogostih težav z e-odkrivanjem, glejte Raziščite, odpravite pogoste težave [z e-odkrivanjem](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)in jih odpravite.
