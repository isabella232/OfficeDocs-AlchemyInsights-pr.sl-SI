---
title: Odpravljanje težav pri pridruženju s hibridnim imenikom Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401923"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Odpravljanje težav pri pridruženju s hibridnim imenikom Azure AD

Zelo priporočamo, da zagotovite, da lahko naprava dostopa do končnih točk registracije naprav pod sistemskim računom tako, da uporabite skript [Preskusite povezljivost registracije naprave](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Če prvič nastavljate registracije naprav, preglejte navodila[uvoda za upravljanje naprav v imeniku Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) in se naučite, kako lahko naprave nadzorujete s storitvijo Azure AD.
1. Če naprave registrirate neposredno v Azure AD [jih včlanite v Intune, se prepričajte, da ste konfigurirali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support)  in imate najprej [licenco](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) za.
1. Zagotovite, da ste pooblaščeni za izvajanje operacij v imeniku Azure AD in imeniku AD na mestu uporabe. Nastavitve za registracije naprav lahko upravlja le globalni skrbnik v imeniku Azure AD. Če želite v imeniku Active Directory na mestu uporabe nastaviti samodejne registracije, morate biti skrbnik imenika Active Directory in storitev AD FS (če je na voljo).

Če želite več informacij o odpravljanju morebitnih težav s hibridnim pridruževanjem, glejte [Odpravljanje težav s hibridnim pridruževanje](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) za nastavitev hibridne naprave, ki so pridružene imeniku Azure AD, in upravljanje naprav s portalom Azure Ad, glejte [Nastavitev hibridne naprave, pridružene imeniku Azure AD (naprave, pridružene domeni na mestu uporabe) v storitvah](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) in [Upravljanje naprav s portalom Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Če želite odpraviti pogoste težave s pridruževanje hibridnim imenikom Azure Active Directory (AD), glejte [Pogosta vprašanja o pridruževanje](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
