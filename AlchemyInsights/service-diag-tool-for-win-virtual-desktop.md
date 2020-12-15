---
title: Orodje za diagnostiko storitve za navidezno namizje sistema Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680232"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Orodje za diagnostiko storitve za navidezno namizje sistema Windows

Windows Virtual Desktop (WVD) ponuja diagnostično orodje, ki omogoča, da skrbniki prepoznajo napake z enim samim vmesnikom. To orodje beleži diagnostične informacije, povezane z diagnostiko, kadar WVD uporablja nekdo, ki je dodelil vlogo WVD. Vsak dnevnik vsebuje informacije o vlogi WVD, ki je vključena v dejavnost, sporočila o napakah, ki se pojavijo med sejo, in informacije o najemniku in uporabniku. Analitika v storitvi Azure log je lahko konfigurirana tako, da zajame dnevnik dejavnosti, ki ga je ustvaril diagnostično orodje. To naredite tako:

1. Ustvarjanje delovnega prostora dnevnika Analytics s [portalom Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ali [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Povežite računalnike s sistemom Windows v storitvi Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Pridobite ID delovnega prostora in primarni ključ delovnega prostora. Čarovnik za nastavitev potrebuje te informacije, da pravilno konfigurira posrednika in zagotovi, da lahko komunicira s storitvijo Azure monitor.
1. [Pritiskajte diagnostične podatke v delovni prostor](https://go.microsoft.com/fwlink/?linkid=2128284). Diagnostične podatke iz WVD najemnika lahko potisnete v analizo dnevnika za delovni prostor.
1. [Prepoznavanje in diagnosticiranje težav](https://go.microsoft.com/fwlink/?linkid=2128338) , ki so notranje ali zunanje glede na WVD.

Če želite izvedeti več o konfiguriranju orodja za diagnostiko storitve za WVD, glejte [Uporaba analitike dnevnika za funkcijo diagnostike](https://go.microsoft.com/fwlink/?linkid=2128084).
