---
title: Odpravljanje težav pri pridruženju imenika Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405761"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Odpravljanje težav pri pridruženju imenika Azure AD

1. Če prvič nastavljate registracije naprav, preverite, ali ste pregledali uvod v upravljanje naprav v imeniku [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) v okviru katere boste dobili navodila, kako naprave pod nadzorom v imenik Azure AD. 
1. Če registrirate naprave neposredno v imeniku Azure AD [in](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) jih včlanite v Intune, morate najprej konfigurirati [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) in imeti licenco.
1. Prepričajte se, da imate dovoljenje za izvajanje operacij v imeniku Azure AD. Nastavitve za registracije naprav lahko upravlja le globalni skrbnik v imeniku Azure AD.
1. Če želite včlanjevati Azure AD, glejte [Načrtovanje pridružite imeniku Azure AD .](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Če želite več podrobnosti o odpravljanju pogostih težav s pridruževanje imeniku Azure AD, glejte Pogosta vprašanja o pridruževanje imeniku [Azure Ad](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) in v napravi s sistemom Windows 10 pro glejte Ni mogoče pridružiti računalniku s sistemom [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) z imenikom Azure AD – nadgradnja na – Microsoftova skupnost
