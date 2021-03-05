---
title: Konfiguracija storitve za zagotavljanje
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484044"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="fe53c-102">Konfiguracija storitve za zagotavljanje</span><span class="sxs-lookup"><span data-stu-id="fe53c-102">Configuring the Provision service</span></span>

<span data-ttu-id="fe53c-103">Za avtomatizirano omogočanje uporabe uporabnika za delo, Azure AD zahteva veljavne poverilnice, ki omogočajo, da se poveže z API-jem spletnih storitev delovnega dne.</span><span class="sxs-lookup"><span data-stu-id="fe53c-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="fe53c-104">Poleg tega je na gumbu» preskusna povezava «na delovnem mestu v programu za omogočanje uporabe uporabnika preverjena tudi veljavnost, če se lahko povežete s posrednikom za omogočanje povezave do storitve Azure AD Connect, ki je povezan z domeno OGLASa.</span><span class="sxs-lookup"><span data-stu-id="fe53c-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="fe53c-105">Če portal Azure vrne napako ob shranjevanju poverilnic, upoštevajte spodnja navodila:</span><span class="sxs-lookup"><span data-stu-id="fe53c-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="fe53c-106">Potrdite, da ste konfigurirali uporabniški račun sistema za integracijo delovnega dne, kot je navedeno v razdelku Vadnica [Konfiguracija uporabnika integracijskega sistema v delovni dan](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="fe53c-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="fe53c-107">Preverite, ali je storitev posrednika za omogočanje povezave s storitvijo Azure AD Connected in se izvaja v strežniku Windows Server s konzolo za upravljanje storitev.</span><span class="sxs-lookup"><span data-stu-id="fe53c-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="fe53c-108">Stanje posrednika na portalu Azure lahko preverite tudi tako, da kliknete gumb ogled posrednika na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="fe53c-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="fe53c-109">Zagotovite, da vnašate vrednost za polje» uporabniško ime za delovni dan «z obliko zapisa username@workday-najemnika.</span><span class="sxs-lookup"><span data-stu-id="fe53c-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="fe53c-110">Če delovni dan – najemnik – ime manjka, preverjanje pristnosti delovnega dne ni uspešno.</span><span class="sxs-lookup"><span data-stu-id="fe53c-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="fe53c-111">Če konfigurirate integracijo z najemnikom izvajanja delovnega dne, si zapomnite načrtovane ure odmore za najemnika delovnega časa.</span><span class="sxs-lookup"><span data-stu-id="fe53c-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="fe53c-112">Delovni dan je načrtovana določitvi časa za svoje najemnike izvajanja čez vikende (po navadi od petka zvečer do sobote zjutraj) in okvare povezljivosti v tem oknu odmore je znana težava, ki samodejno razreši takoj, ko so najemniki implementacije spet v spletu.</span><span class="sxs-lookup"><span data-stu-id="fe53c-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="fe53c-113">V redkih primerih se lahko prikaže tudi to sporočilo o napaki, če se je geslo uporabnika sistema integracije spremenilo zaradi osveževanja najemnika ali če je račun v zaklenjenem ali poteklem stanju.</span><span class="sxs-lookup"><span data-stu-id="fe53c-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="fe53c-114">Preverite stanje uporabnika sistema integracije s skrbnikom delovnega dne.</span><span class="sxs-lookup"><span data-stu-id="fe53c-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="fe53c-115">Če želite več informacij o konfiguriranju delovnega dne za avtomatizirano omogočanje uporabe, glejte [Vadnica: konfiguracija delovnega dne za samodejno omogočanje uporabe uporabnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="fe53c-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
