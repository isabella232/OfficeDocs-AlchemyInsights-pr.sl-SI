---
title: Iskanje dogodkov, izvedenih v pravilih za mapo» Prejeto «
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483704"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="81c5e-102">Iskanje dogodkov, izvedenih v pravilih za mapo» Prejeto «</span><span class="sxs-lookup"><span data-stu-id="81c5e-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="81c5e-103">Ko so pravila za mapo» Prejeto «ustvarjena, spremenjena ali izbrisana, so dogodki zapisani v dnevniku nadzora.</span><span class="sxs-lookup"><span data-stu-id="81c5e-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="81c5e-104">Oglejte si navodila za pregled:</span><span class="sxs-lookup"><span data-stu-id="81c5e-104">Here's how to review them:</span></span>

1. <span data-ttu-id="81c5e-105">Obiščite središče za [skladnost z varnostnim &om sistema Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="81c5e-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="81c5e-106">Izberite Išči > nadzor dnevnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="81c5e-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="81c5e-107">Če opazite obvestilo, ki ga morate vklopiti, ga vklopite zdaj.</span><span class="sxs-lookup"><span data-stu-id="81c5e-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="81c5e-108">Če ta funkcija ni vklopljena, rezultati iskanja ne bodo mogli povleči podatkov iz prejšnjih datumov.</span><span class="sxs-lookup"><span data-stu-id="81c5e-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="81c5e-109">Izberite polje dejavnosti in poiščite dejavnosti nabiralnika strežnika Exchange, nato pa v programu Outlook Web App izberite New-InboxRule ustvari pravilo za mapo» Prejeto «.</span><span class="sxs-lookup"><span data-stu-id="81c5e-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="81c5e-110">Ko končate, kliknite zunaj podokna, da minimirate podokno dejavnosti.</span><span class="sxs-lookup"><span data-stu-id="81c5e-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="81c5e-111">Določite datumski obseg in nato v polju uporabniki izberite uporabniško ime za uporabnika, ki ga želite raziskati.</span><span class="sxs-lookup"><span data-stu-id="81c5e-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="81c5e-112">Izberete lahko več uporabnikov hkrati.</span><span class="sxs-lookup"><span data-stu-id="81c5e-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="81c5e-113">Izberite Išči.</span><span class="sxs-lookup"><span data-stu-id="81c5e-113">Select Search.</span></span> <span data-ttu-id="81c5e-114">Dejavnosti so prikazane v razdelku Rezultati.</span><span class="sxs-lookup"><span data-stu-id="81c5e-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="81c5e-115">Če si želite ogledati podrobnosti, izberite dejavnost in nato izberite več informacij.</span><span class="sxs-lookup"><span data-stu-id="81c5e-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="81c5e-116">V razdelku parametri si lahko ogledate ime pravila, nabora pogojev in dejanja, ki jih bo pravilo sprejelo.</span><span class="sxs-lookup"><span data-stu-id="81c5e-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="81c5e-117">Če želite izvedeti več, glejte Iskanje v dnevniku nadzora sistema Office 365 za odpravljanje pogostih scenarijev.</span><span class="sxs-lookup"><span data-stu-id="81c5e-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>