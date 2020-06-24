---
title: Uporaba pravilnikov PowerShell za skupno rabo in odnosov organizacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862156"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Uporaba pravilnikov PowerShell za skupno rabo in odnosov organizacije


Za odnose organizacije preglejte podrobne podatke o skladnji in parametrih za: [pridobite-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-organizationrelacija](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [set-Organizationrelacija](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) in [Odstrani-organizationrelacija](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Če želite ustvariti pravilnik za skupno rabo, uporabite [novo pravilnik](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Če želite [uporabiti pravilnik o skupni rabi za nabiralnik ali uporabnika](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) , morate uporabiti kombinacijo [set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) in [zaslužiti-poštni nabiralnik](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) z novo ustvarjeno politiko. V [ublažiti, onesposobiti ali premestitev a črepina zvitost](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) vi potreba rabiti [število enakih oseb-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ter [premestitev-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Za popolno razumevanje te teme preberite:**

[Skupna raba v Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)