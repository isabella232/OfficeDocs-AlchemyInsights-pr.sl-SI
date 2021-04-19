---
title: Dogodki v živo v Yammer napakah pri ustvarjanju
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825531"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="10f10-102">Dogodki v živo v Yammer napakah pri ustvarjanju</span><span class="sxs-lookup"><span data-stu-id="10f10-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="10f10-103">**Ustvarjanje dogodkov v živo v Yammer**</span><span class="sxs-lookup"><span data-stu-id="10f10-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="10f10-104">Yammer bo prikazala možnost za ustvarjanje dogodka v živo ves čas.</span><span class="sxs-lookup"><span data-stu-id="10f10-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="10f10-105">V nekaterih primerih uporabnik morda ne bo izpolnjeval pogojev za ustvarjanje dogodka v živo in prejel napako, ko jo bo poskusil ustvariti.</span><span class="sxs-lookup"><span data-stu-id="10f10-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="10f10-106">V spodnjih napravah so navedeni pogosti razlogi za to težavo in ponudijo načine, kako lahko to razrešite pri končnih uporabnikih.</span><span class="sxs-lookup"><span data-stu-id="10f10-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="10f10-107">**Kdo lahko ustvarja dogodke v živo**</span><span class="sxs-lookup"><span data-stu-id="10f10-107">**Who can create live events**</span></span>
- <span data-ttu-id="10f10-108">Licenca za Office 365 Enterprise E1, E3 ali E5 ali licenca za Office 365 a3 ali a5.</span><span class="sxs-lookup"><span data-stu-id="10f10-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="10f10-109">Dovoljenje za ustvarjanje dogodkov v živo v skrbniškem središču za Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="10f10-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="10f10-110">Dovoljenje za ustvarjanje dogodkov v živo v Microsoft Stream (za dogodke, ki so bili ustvarjeni z zunanjo aplikacijo ali napravo za oddajanje).</span><span class="sxs-lookup"><span data-stu-id="10f10-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="10f10-111">Polnopravna članstva v skupini organizacije (ne sme biti gost ali iz druge organizacije).</span><span class="sxs-lookup"><span data-stu-id="10f10-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="10f10-112">Privatno načrtovanje sestanka, skupna raba zaslona in skupna raba videa v storitvi IP, vklopljeno v pravilniku za sestanek Team.</span><span class="sxs-lookup"><span data-stu-id="10f10-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="10f10-113">**Pravilniki za ustvarjanje dogodkov v živo**</span><span class="sxs-lookup"><span data-stu-id="10f10-113">**Live event creation policies**</span></span>

<span data-ttu-id="10f10-114">Yammer sledi pravilnikom o dogodku v živo, ki je nastavljen v najemniku sistema Office 365 za Stream.</span><span class="sxs-lookup"><span data-stu-id="10f10-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="10f10-115">Privzeto lahko vsi v vaši organizaciji ustvarijo dogodek v živo.</span><span class="sxs-lookup"><span data-stu-id="10f10-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="10f10-116">Skrbniki lahko [spremenijo to nastavitev, kar lahko uporabnikom prepreči, da bi ustvarili](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)dogodkov v živo.</span><span class="sxs-lookup"><span data-stu-id="10f10-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="10f10-117">Pomembno je, da preverite, ali imajo uporabniki dovoljenja za ustvarjanje dogodkov v živo, če prejmejo napako pravilnika.</span><span class="sxs-lookup"><span data-stu-id="10f10-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
