---
title: Odpravljanje težav z včlaninjem naprav s sistemom Android Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008094"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Odpravljanje težav z včlaninjem naprav s sistemom Android Microsoft Intune

Preglejte vire spodaj, da odpravite težavo.
  
Nekatere pogoste težave in koraki za odpravljanje težav:
  
 **Napaka »Naprava ni šifrirana« v Company Portal:** Novejše različice sistema Android, ki se začnejo s sistemom v7.0, zahtevajo zagonsko geslo, s tem pa se prepričate, da je naprava v celoti šifrirana. Običajne rešitve so, da omogočite pripenjanje pin-a ob zagonu ali v celoti šifrirate napravo. Preglejte [ta dokument,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) če želite več informacij.
  
 Naprave se ne prijavijo v storitvi Intune ali pa so v skrbniški konzoli **za Intune prikazane kot »neprimerne«:** Nekateri napravi Samsung 4.4 in 5.5 se morda ne prijavita v storitev. Za to težavo so na voljo 3 rešitve:
  
1. Ročno odprite aplikacijo Intune Company Portal, ki samodejno zažene sinhronizacijo naprave.

2. Posodobite napravo na Android 6.0 ali višjo različico.

3. Onemogočite samsung Smart Managerju upravljanje Intune Company Portal. Preglejte [ta](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) dokument, če želite dodatne podrobnosti o teh težavah in rešitve.

 **Vrsta uporabniške licence Neveljavna** ali Uporabniško ime ni **prepoznano:** uporabniku mora biti dodeljena licenca za Intune ali EMS. Preglejte te dokumente, da dodelite licenco prek: Office skrbniškega središča ali portala Azure.
  
Dodatni viri za odpravljanje težave:
  
1. S [portalom za odpravljanje težav za Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lahko diagnosticirate in odpravite pogoste napake z včlani. Preglejte [ta dokument,](https://docs.microsoft.com/intune/help-desk-operators) če želite več podrobnosti.

2. V [tem dokumentu](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) si oglejte seznam pogostih napak, ki preprečujejo včlanitev in rešitve za posamezne uporabnike.

3. [Preberite, kako včlanite naprave s sistemom Android Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
