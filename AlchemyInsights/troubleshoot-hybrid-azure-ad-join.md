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
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="3b0f4-102">Odpravljanje težav pri pridruženju s hibridnim imenikom Azure AD</span><span class="sxs-lookup"><span data-stu-id="3b0f4-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="3b0f4-103">Zelo priporočamo, da zagotovite, da lahko naprava dostopa do končnih točk registracije naprav pod sistemskim računom tako, da uporabite skript [Preskusite povezljivost registracije naprave](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="3b0f4-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="3b0f4-104">Če prvič nastavljate registracije naprav, preglejte navodila[uvoda za upravljanje naprav v imeniku Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) in se naučite, kako lahko naprave nadzorujete s storitvijo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b0f4-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="3b0f4-105">Če naprave registrirate neposredno v Azure AD [jih včlanite v Intune, se prepričajte, da ste konfigurirali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support)  in imate najprej [licenco](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) za.</span><span class="sxs-lookup"><span data-stu-id="3b0f4-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="3b0f4-106">Zagotovite, da ste pooblaščeni za izvajanje operacij v imeniku Azure AD in imeniku AD na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="3b0f4-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="3b0f4-107">Nastavitve za registracije naprav lahko upravlja le globalni skrbnik v imeniku Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b0f4-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="3b0f4-108">Če želite v imeniku Active Directory na mestu uporabe nastaviti samodejne registracije, morate biti skrbnik imenika Active Directory in storitev AD FS (če je na voljo).</span><span class="sxs-lookup"><span data-stu-id="3b0f4-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="3b0f4-109">Če želite več informacij o odpravljanju morebitnih težav s hibridnim pridruževanjem, glejte [Odpravljanje težav s hibridnim pridruževanje](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) za nastavitev hibridne naprave, ki so pridružene imeniku Azure AD, in upravljanje naprav s portalom Azure Ad, glejte [Nastavitev hibridne naprave, pridružene imeniku Azure AD (naprave, pridružene domeni na mestu uporabe) v storitvah](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) in [Upravljanje naprav s portalom Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3b0f4-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="3b0f4-110">Če želite odpraviti pogoste težave s pridruževanje hibridnim imenikom Azure Active Directory (AD), glejte [Pogosta vprašanja o pridruževanje](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="3b0f4-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
