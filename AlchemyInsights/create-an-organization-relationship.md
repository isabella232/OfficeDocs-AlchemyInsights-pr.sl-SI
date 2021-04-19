---
title: Ustvarjanje odnosa organizacije, ki uporabnikom omogoča sodelovanje z drugo organizacijo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816144"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="f9273-102">Ustvarjanje odnosa organizacije, ki uporabnikom omogoča sodelovanje z drugo organizacijo</span><span class="sxs-lookup"><span data-stu-id="f9273-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="f9273-103">Na nadzorni plošči Skrbniškega središča za Microsoft 365 odprite razdelek **Skrbnik** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="f9273-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="f9273-104">Pomaknite se v razdelek **Organizacija** > **Skupna raba**.</span><span class="sxs-lookup"><span data-stu-id="f9273-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="f9273-105">V **razdelku Skupna raba** organizacije kliknite **Novo.**</span><span class="sxs-lookup"><span data-stu-id="f9273-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="f9273-106">V **novem odnosu** organizacije v **polje Ime** relacije vnesite prijazno ime za odnos organizacije.</span><span class="sxs-lookup"><span data-stu-id="f9273-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="f9273-107">V polje **Domains to share with** (Domene za skupno rabo) vnesite domeno za zunanjo organizacijo v storitvi Office 365 ali Exchange na mestu uporabe, kjer želite, da vaši koledarji vidijo.</span><span class="sxs-lookup"><span data-stu-id="f9273-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="f9273-108">Če morate vnesti več domen, imena domen ločite z vejico.</span><span class="sxs-lookup"><span data-stu-id="f9273-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="f9273-109">Na primer contoso.com service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="f9273-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="f9273-110">Potrdite potrditveno **polje Omogoči skupno rabo informacij o prostem/zasedenem** času na koledarju, da vklopite skupno rabo koledarja z domenami, ki ste jih navedeni.</span><span class="sxs-lookup"><span data-stu-id="f9273-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="f9273-111">Nastavite raven skupne rabe za podatke o prostem/zasedenem času na koledarju in nastavite, kateri uporabniki lahko dajo v skupno rabo informacije o prostem/zasedenem času koledarja.</span><span class="sxs-lookup"><span data-stu-id="f9273-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="f9273-112">Če želite nastaviti raven dostopa »prosto/zasedeno« izberite nekaj od tega:</span><span class="sxs-lookup"><span data-stu-id="f9273-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="f9273-113">**Samo podatki o prostem/zasedenem času v koledarju**</span><span class="sxs-lookup"><span data-stu-id="f9273-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="f9273-114">**Koledar : prosto/zasedeno s časom, zadevo in lokacijo**</span><span class="sxs-lookup"><span data-stu-id="f9273-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="f9273-115">Če želite nastaviti, kateri uporabniki bodo v skupno rabo dali informacije o prostem/zasedenem času na koledarju, izberite nekaj od tega:</span><span class="sxs-lookup"><span data-stu-id="f9273-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="f9273-116">**Vsi v vaši organizaciji**</span><span class="sxs-lookup"><span data-stu-id="f9273-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="f9273-117">**Določena varnostna skupina**</span><span class="sxs-lookup"><span data-stu-id="f9273-117">**A specified security group**</span></span>  

<span data-ttu-id="f9273-118">Kliknite **prebrskaj,** da na seznamu izberete varnostno skupino, nato pa kliknite V **redu.**</span><span class="sxs-lookup"><span data-stu-id="f9273-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="f9273-119">Kliknite **shrani,** da ustvarite odnos organizacije.</span><span class="sxs-lookup"><span data-stu-id="f9273-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="f9273-120">**Opomba:** Konfiguracije v več najemnikih ne podpirajo osebnih stikov za iskanje prostega/zasedenega časa.</span><span class="sxs-lookup"><span data-stu-id="f9273-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="f9273-121">Če želite, da iskanje prostega/zasedenega časa deluje, morajo biti stiki vključeni na globalni seznam naslovov.</span><span class="sxs-lookup"><span data-stu-id="f9273-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="f9273-122">**Za podrobne informacije o tej temi preberite:**</span><span class="sxs-lookup"><span data-stu-id="f9273-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="f9273-123">Ustvarjanje odnosa organizacije v Exchange Onlineu</span><span class="sxs-lookup"><span data-stu-id="f9273-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="f9273-124">Spreminjanje odnosa organizacije v Exchange Onlineu</span><span class="sxs-lookup"><span data-stu-id="f9273-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="f9273-125">Odstranjevanje odnosa organizacije v Exchange Onlineu</span><span class="sxs-lookup"><span data-stu-id="f9273-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
