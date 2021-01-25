---
title: Preslikava atributov uporabnika za omogočanje uporabe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949896"
---
# <a name="user-provisioning-attribute-mapping"></a>Preslikava atributov uporabnika za omogočanje uporabe

1. Za odpravljanje težav z znanimi težavami pri preslikavi atributov glejte [preslikave atributov](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) zagotavlja podporo za omogočanje uporabe uporabnika za aplikacije SaaS, kot je platforme Salesforce, G Suite in drugi. Če omogočite omogočanje uporabe uporabnika za uporabo storitve SaaS, portal Azure nadzoruje svoje vrednosti atributov prek preslikav atributov. Če želite izvedeti, kako prilagodite privzete preslikave atributov, si oglejte [prilagajanje atributov za omogočanje uporabe uporabnikov v storitvi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Če želite izvedeti več o omogočanju uporabe uporabnikov aplikacije SaaS, glejte [Kaj je avtomatizirano omogočanje uporabe uporabnikov v storitvi AZURE ad?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Ko prilagodite preslikave atributov za omogočanje uporabe uporabnika, boste morda ugotovili, da atribut, ki ga želite preslikati, ni prikazan na seznamu izvorni atribut. [Sinhronizacija atributa iz imenika Active Directory v storitvi AZURE ad za omogočanje uporabe v članku aplikacije](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) vam pokaže, kako dodati manjkajoči atribut tako, da ga sinhronizirate z oglasa na mestu uporabe v storitvi Azure ad.
