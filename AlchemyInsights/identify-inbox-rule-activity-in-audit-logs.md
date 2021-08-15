---
title: Prepoznavanje dejavnosti pravila nabiralnika v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976881"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Prepoznavanje dejavnosti pravila nabiralnika v dnevnikih nadzora

Z iskanjem v dnevniku nadzora v središču za varnost in skladnost & s predpisi storitve Microsoft 365 si lahko ogledate dogodke pravila nabiralnika (ustvarjanje, spreminjanje in brisanje pravil nabiralnika).

1. Prijavite se v središče [za Microsoft 365 s predpisi.](https://protection.office.com/)

2. Pojdite na stran **iskanja**  >  **v dnevniku nadzora** iskanja.

3. Izberite datumski obseg v **poljih Začetni datum** in **Končni** datum.

4. V **Exchange nabiralnika** preverite,  ali je polje Dejavnosti nastavljeno na **New-InboxRule Create/modify/enable/disable Inbox rule**.

5. Kliknite **Iskanje.**

Med rezultati izberite zapis nadzora. V oknu s podrobnostmi kliknite **Več informacij.** Informacije o nastavitvah pravila za mapo »Prejeto« so prikazane v **polju Parametri.**

Če želite več informacij, glejte [Določanje, ali je uporabnik ustvaril pravilo za mapo »Prejeto«](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
