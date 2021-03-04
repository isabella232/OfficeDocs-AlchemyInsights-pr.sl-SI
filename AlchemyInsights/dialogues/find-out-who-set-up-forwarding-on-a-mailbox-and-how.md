---
title: Ugotovite, kdo je nastavil posredovanje v nabiralniku in kako
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429995"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="caed9-102">Ugotovite, kdo je nastavil posredovanje v nabiralniku in kako</span><span class="sxs-lookup"><span data-stu-id="caed9-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="caed9-103">Če je bila zunanja preusmeritev nastavljena na nabiralnik, je dejavnost revidirana kot del ukaza» cmdlet «Set-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="caed9-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="caed9-104">To storite tako, da poiščete dejavnost v dnevniku nadzora:</span><span class="sxs-lookup"><span data-stu-id="caed9-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="caed9-105">Obiščite središče za [skladnost z varnostnim &om sistema Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="caed9-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="caed9-106">Izberite  >  **iskanje dnevnika nadzora** iskanja.</span><span class="sxs-lookup"><span data-stu-id="caed9-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="caed9-107">Če opazite obvestilo, ki ga morate vklopiti, ga vklopite zdaj.</span><span class="sxs-lookup"><span data-stu-id="caed9-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="caed9-108">Če ta funkcija ni vklopljena, rezultati iskanja ne bodo mogli povleči podatkov iz prejšnjih datumov.</span><span class="sxs-lookup"><span data-stu-id="caed9-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="caed9-109">Prepričajte se, da je polje **dejavnosti** nastavljeno tako, da **prikaže rezultate za vse dejavnosti** (privzeto).</span><span class="sxs-lookup"><span data-stu-id="caed9-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="caed9-110">Določite datumski obseg.</span><span class="sxs-lookup"><span data-stu-id="caed9-110">Specify the date range.</span></span> <span data-ttu-id="caed9-111">Ni vam treba določiti uporabniškega imena.</span><span class="sxs-lookup"><span data-stu-id="caed9-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="caed9-112">Izberite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="caed9-112">Select **Search**.</span></span> <span data-ttu-id="caed9-113">Dejavnosti so prikazane v razdelku **Rezultati**.</span><span class="sxs-lookup"><span data-stu-id="caed9-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="caed9-114">Izberite **Rezultati filtra** in vnesite **nabiralnik** v polje Filter **dejavnosti** .</span><span class="sxs-lookup"><span data-stu-id="caed9-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="caed9-115">To vrne vse dejavnosti **nabora nabiralnika** .</span><span class="sxs-lookup"><span data-stu-id="caed9-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="caed9-116">Če si želite ogledati podrobnosti, izberite dejavnost in nato izberite **več informacij**.</span><span class="sxs-lookup"><span data-stu-id="caed9-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="caed9-117">V razdelku **Parametri** si lahko ogledate e-poštni naslov posredovanja, ki je bil nastavljen v nabiralniku.</span><span class="sxs-lookup"><span data-stu-id="caed9-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="caed9-118">**ID** uporabnika predstavlja uporabnika, ki je nastavil zunanjo posredovanje v nabiralniku.</span><span class="sxs-lookup"><span data-stu-id="caed9-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="caed9-119">Če želite izvedeti več, glejte [Iskanje v dnevniku nadzora sistema Office 365 za odpravljanje pogostih scenarijev](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="caed9-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>