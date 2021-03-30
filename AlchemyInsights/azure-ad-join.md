---
title: Pridružitev imeniku Azure Active Directory
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
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405672"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="8a88b-102">Pridružitev imeniku Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="8a88b-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="8a88b-103">Če prvič nastavljate registracije naprav, preverite, ali ste pregledali uvod v upravljanje naprav v imeniku [Azure Active Directory,](/azure/active-directory/devices/overview) v okviru katere boste dobili navodila, kako naprave pod nadzorom v imenik Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a88b-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="8a88b-104">Če registrirate naprave neposredno v imeniku Azure AD [in](/mem/intune/fundamentals/licenses-assign) jih včlanite v Intune, morate najprej konfigurirati [Intune](/mem/intune/enrollment/device-enrollment) in imeti licenco.</span><span class="sxs-lookup"><span data-stu-id="8a88b-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="8a88b-105">Prepričajte se, da imate dovoljenje za izvajanje operacij v imeniku Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a88b-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="8a88b-106">Nastavitve za registracije naprav lahko upravlja le globalni skrbnik v imeniku Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a88b-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="8a88b-107">Če želite včlanjevati Azure AD, glejte [Načrtovanje pridružite imeniku Azure AD .](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="8a88b-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="8a88b-108">Če želite več podrobnosti o odpravljanju pogostih težav s pridruževanje imenikom Azure AD, glejte Pogosta vprašanja o pridruževanje imeniku [Azure Ad](/azure/active-directory/devices/faq) in v napravi s sistemom Windows 10 pro glejte Ni se mogoče pridružiti računalniku s sistemom [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)z imenikom Azure AD – nadgradnja na – Microsoftova skupnost.</span><span class="sxs-lookup"><span data-stu-id="8a88b-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
