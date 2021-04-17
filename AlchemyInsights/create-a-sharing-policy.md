---
title: Ustvarite pravilnik o skupni rabi, da lahko uporabniki dajo koledar v skupno rabo z osebami zunaj organizacije
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
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816288"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="7b43f-102">Ustvarite pravilnik o skupni rabi, da lahko uporabniki dajo koledar v skupno rabo z osebami zunaj organizacije</span><span class="sxs-lookup"><span data-stu-id="7b43f-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="7b43f-103">Na nadzorni plošči Skrbniškega središča za Microsoft 365 odprite razdelek **Skrbnik** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="7b43f-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="7b43f-104">Pomaknite se v razdelek **Organizacija** > **Skupna raba**.</span><span class="sxs-lookup"><span data-stu-id="7b43f-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="7b43f-105">V pogledu seznama v razdelku **Posamezna skupna raba** kliknite **Novo** .</span><span class="sxs-lookup"><span data-stu-id="7b43f-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="7b43f-106">V razdelku **Nov pravilnik o skupni rabi** vnesite prijazno ime za pravilnik o skupni rabi v polje **Ime pravilnika**.</span><span class="sxs-lookup"><span data-stu-id="7b43f-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="7b43f-107">Kliknite **Dodaj**, da določite pravila skupne rabe za ta pravilnik.</span><span class="sxs-lookup"><span data-stu-id="7b43f-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="7b43f-108">V razdelku **Pravilo skupne rabe** izberite eno od teh možnosti, da določite domene, za katere želite omogočiti skupno rabo:</span><span class="sxs-lookup"><span data-stu-id="7b43f-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="7b43f-109">**Skupna raba z vsemi domenami**</span><span class="sxs-lookup"><span data-stu-id="7b43f-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="7b43f-110">**Skupna raba z določeno domeno**</span><span class="sxs-lookup"><span data-stu-id="7b43f-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="7b43f-111">Če izberete **Skupna raba z določeno domeno**, vnesite ime domene, za katero želite omogočiti skupno rabo.</span><span class="sxs-lookup"><span data-stu-id="7b43f-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="7b43f-112">Če želite vnesti več domen za ta pravilnik o skupni rabi, shranite nastavitve za prvo domeno, nato pa uredite pravila skupne rabe, da dodate več domen.</span><span class="sxs-lookup"><span data-stu-id="7b43f-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="7b43f-113">Če želite določiti vrsto informacij za skupno rabo, potrdite polje **Skupna raba mape koledarja**, nato pa izberite eno od teh možnosti:</span><span class="sxs-lookup"><span data-stu-id="7b43f-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="7b43f-114">**Samo podatki o prostem/zasedenem času v koledarju**</span><span class="sxs-lookup"><span data-stu-id="7b43f-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="7b43f-115">**Podatki o prostem/zasedenem času, zadevi in lokaciji v koledarju**</span><span class="sxs-lookup"><span data-stu-id="7b43f-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="7b43f-116">**Vsi podatki o sestankih v koledarju, vključno s časom, zadevo, lokacijo in naslovom**</span><span class="sxs-lookup"><span data-stu-id="7b43f-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="7b43f-117">Kliknite **Shrani**, da nastavite pravila za pravilnik o skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="7b43f-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="7b43f-118">Če želite nastaviti ta pravilnik kot novi privzeti pravilnik o skupni rabi za vse uporabnike v organizaciji, potrdite polje **Omogoči ta pravilnik kot privzeti pravilnik o skupni rabi**.</span><span class="sxs-lookup"><span data-stu-id="7b43f-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="7b43f-119">Kliknite **Shrani**, da ustvarite pravilnik o skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="7b43f-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="7b43f-120">**Za podrobne informacije o tej temi preberite:**</span><span class="sxs-lookup"><span data-stu-id="7b43f-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="7b43f-121">Ustvarjanje pravilnika o skupni rabi v storitvi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="7b43f-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="7b43f-122">Uporaba pravilnika o skupni rabi za nabiralnike v storitvi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="7b43f-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="7b43f-123">Spreminjanje, onemogočanje ali odstranjevanje pravilnika o skupni rabi v storitvi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="7b43f-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)