---
title: Težava z varnostnimi skupinami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177633"
---
# <a name="issue-with-security-groups"></a>Težava z varnostnimi skupinami

**Če prihaja do napake v omrežju AADDS104**

Neveljavna pravila skupine za varnost omrežja so najpogostejši vzrok za napake omrežja za domenske storitve Azure Active Directory (AD DS). Skupina za varnost omrežja za navidezno omrežje mora omogočati dostop do določenih vrat in protokolov. Če so ta vrata blokirana, platforma Azure ne more nadzorovati ali posodobiti upravljane domene. Vpliva tudi sinhronizacija med storitvijo Azure AD in Azure AD DS. Zagotovite, da so privzeta vrata odprta, da se izognete prekinitvi v storitvi.

Če želite razumeti in razrešiti pogosta opozorila za težave s konfiguracijo omrežja za varnost, glejte [Dodajanje in preverjanje varnostnih skupin](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
