---
title: 932 nadgradnja AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766509"
---
# <a name="upgrade-azure-ad-connect"></a>Nadgradnja povezave Azure AD Connect

Samodejna nadgradnja je privzeto omogočena za Azure AD Connect, ki pomaga zagotoviti, da uporabljate najnovejšo različico. Če želite preveriti samodejne nastavitve nadgradnje, uporabite ukaz» cmdlet « **Get-ADSyncAutoUpgrade** v POWERSHELL Azure ad. Ukaz» cmdlet «bo vrnil eno od naslednjih vrednosti:

- **Omogočeno**: Samodejna nadgradnja je omogočena.

- **Onemogočeno**: Samodejna nadgradnja je onemogočena.

- **Prekinjena**: sistem ni več upravičen do samodejnega nadgrajevanja. Te vrednosti ni mogoče konfigurirati; je nastavljen s sistemom.

Če želite več informacij, glejte [Samodejna nadgradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Če želite prenesti najnovejšo različico Azure AD Connect, pojdite na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
