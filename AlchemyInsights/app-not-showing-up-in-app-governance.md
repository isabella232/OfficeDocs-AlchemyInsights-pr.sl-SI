---
title: Moja aplikacija ni prikazana v upravljanju aplikacij
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454990"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Moja aplikacija ni prikazana v upravljanju aplikacij

Če vaša aplikacija ni prikazana v upravljanje aplikacij, preverite to:

1. Odprite [Azure AD](https://aad.portal.azure.com/) in poiščite ID aplikacije, tako da poiščete ime aplikacije v zgornji vrstici na strani Pregled.

1. Dostopajte Graph Raziskovalcu in poiščite ID aplikacije v glavnem imenu storitve, tako da uporabite to poizvedbo in jo zamenjate z ustreznim ID-jem <appId> aplikacije: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Če ni vrnjen noben rezultat, s to poizvedbo poiščite ID aplikacije in ga zamenjajte z ustreznim ID-jem <appId> aplikacije: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Če pride do težav s poizvedbo, glejte [Dobite podporo.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Če želite več informacij ali vpogleda v aplikacije v upravljanju aplikacij, glejte [Več informacij o vidljivosti in vpogledih.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Če želite več informacij o ogledu aplikacij, [glejte Ogled aplikacij.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
