---
title: 932 nadgradnja AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806055"
---
# <a name="upgrade-azure-ad-connect"></a>Nadgradnja povezave s storitvijo Azure AD

Samodejno nadgradnja je privzeto omogočena za povezavo s storitvijo Azure AD Connect, ki zagotavlja, da izvajate najnovejšo različico. Če želite preveriti nastavitve samodejne nadgradnje, uporabite ukaz» cmdlet « **Get-ADSyncAutoUpgrade** v storitvi Azure ad PowerShell. Ukaz» cmdlet «bo vrnil eno od teh vrednosti:

- **Omogočeno**: omogočena je Samodejna nadgradnja.

- **Onemogočeno**: Samodejna nadgradnja je onemogočena.

- **Začasno ustavljeno**: sistem ni več upravičen do samodejnega posodabljanja. Te vrednosti ni mogoče konfigurirati; sistem je nastavljen s sistemom.

Če želite več informacij, glejte [Samodejna nadgradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Če želite prenesti najnovejšo različico storitve Azure AD Connect, pojdite na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
