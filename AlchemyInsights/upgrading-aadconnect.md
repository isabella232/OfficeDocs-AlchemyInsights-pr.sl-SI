---
title: Nadgradnja povezave AADConnect 932
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
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104828"
---
# <a name="upgrade-azure-ad-connect"></a>Nadgradnja storitve Azure AD Povezovalnik

Samodejna nadgradnja je privzeto omogočena za imenik Azure AD Povezovalnik ki pomaga zagotoviti, da imate nameščeno najnovejšo različico. Če želite preveriti nastavitve samodejne nadgradnje, uporabite ukaz »cmdlet« **Get-ADSyncAutoUpgrade** v azure AD PowerShell. Ukaz »cmdlet« vrne eno od teh vrednosti:

- **Omogočeno:** Samodejna nadgradnja je omogočena.

- **Onemogočeno:** Samodejna nadgradnja je onemogočena.

- **Začasno** prekinjeno: sistem ni več upravičen do samodejne nadgradnje. Te vrednosti ne morete konfigurirati; nastavil sistem.

Če želite več informacij, glejte [Samodejna nadgradnja.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Če želite prenesti najnovejšo različico imenika Azure AD Povezovalnik, odprite [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
