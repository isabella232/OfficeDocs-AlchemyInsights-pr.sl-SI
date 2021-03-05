---
title: Branje dnevnikov nadzora za izbrisane dogodke
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483318"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="0b9d5-102">Branje dnevnikov nadzora za izbrisane dogodke</span><span class="sxs-lookup"><span data-stu-id="0b9d5-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="0b9d5-103">To naredite tako:</span><span class="sxs-lookup"><span data-stu-id="0b9d5-103">Here's how to do this:</span></span>

1. <span data-ttu-id="0b9d5-104">Obiščite središče za [skladnost z varnostnim &om sistema Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="0b9d5-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="0b9d5-105">Izberite   >  [**iskanje dnevnika nadzora**](https://go.microsoft.com/fwlink/?linkid=2103759)iskanja.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="0b9d5-106">Če se prikaže obvestilo, ki ga morate vklopiti, ga vklopite zdaj.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="0b9d5-107">Če funkcija ni vklopljena, rezultati iskanja ne bodo mogli povleči podatkov iz prejšnjih datumov.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="0b9d5-108">Izberite **dejavnosti** in poiščite **dejavnosti nabiralnika** v strežniku Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="0b9d5-109">Izberite **izbrisana sporočila iz mape» Izbrisano** «in **premaknjena sporočila v** možnosti mape» Izbrisano «.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="0b9d5-110">Ko končate, kliknite zunaj podokna, da minimirate podokno **dejavnosti** .</span><span class="sxs-lookup"><span data-stu-id="0b9d5-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="0b9d5-111">Določite datumski obseg in nato v polju **Uporabniki** izberite uporabniško ime za uporabnika, ki ga želite raziskati.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="0b9d5-112">Izberete lahko več uporabnikov hkrati.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="0b9d5-113">Izberite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-113">Select **Search**.</span></span> <span data-ttu-id="0b9d5-114">Dejavnosti so prikazane v razdelku **Rezultati**.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="0b9d5-115">Če si želite ogledati podrobnosti, izberite dejavnost in nato izberite **več informacij**.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="0b9d5-116">Dodatne informacije o izbrisanem elementu, na primer vrstici» zadeva «in mestu elementa, ko je bila izbrisana, so prikazane v polju» **AffectedItems** «.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="0b9d5-117">Izbrisanih elementov ni mogoče obnoviti s funkcijo dnevnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="0b9d5-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="0b9d5-118">Če želite obnoviti izbrisane elemente, glejte [obnovitev izbrisanih elementov ali e-pošte v programu Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="0b9d5-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="0b9d5-119">Če želite izvedeti več, glejte [Iskanje v dnevniku nadzora sistema Office 365 za odpravljanje pogostih scenarijev](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="0b9d5-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
