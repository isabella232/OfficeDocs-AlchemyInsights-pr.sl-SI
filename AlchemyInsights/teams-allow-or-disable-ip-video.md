---
title: Teams allow or disable IP video
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
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826359"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="d83fd-102">Teams allow or disable IP video</span><span class="sxs-lookup"><span data-stu-id="d83fd-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="d83fd-103">**Spreminjanje ali ustvarjanje pravilnika srečanja**</span><span class="sxs-lookup"><span data-stu-id="d83fd-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="d83fd-104">Če želite spremeniti ali ustvariti pravilnik srečanja, pojdite v skrbniško središče za Microsoft Teams in **> Srečanja > Srečanja.**</span><span class="sxs-lookup"><span data-stu-id="d83fd-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="d83fd-105">Na seznamu izberite pravilnik ali kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="d83fd-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="d83fd-106">Če ustvarjate nov pravilnik, dodajte ime in opis.</span><span class="sxs-lookup"><span data-stu-id="d83fd-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="d83fd-107">V imenu ne sme biti posebnih znakov, ime pa ne sme biti daljše od 64 znakov.</span><span class="sxs-lookup"><span data-stu-id="d83fd-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="d83fd-108">Izberite nastavitve in kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="d83fd-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="d83fd-109">Recimo, da imate veliko uporabnikov in želite omejiti količino pasovne širine, ki bi jo srečanje zahtevalo.</span><span class="sxs-lookup"><span data-stu-id="d83fd-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="d83fd-110">Ustvarite nov pravilnik po meri, imenovan »Omejena pasovna širina« in onemogočite te nastavitve:</span><span class="sxs-lookup"><span data-stu-id="d83fd-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="d83fd-111">V razdelku **Zvok in video**:</span><span class="sxs-lookup"><span data-stu-id="d83fd-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="d83fd-112">Izklopite možnost »Dovoli snemanje v oblaku«.</span><span class="sxs-lookup"><span data-stu-id="d83fd-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="d83fd-113">Izklopite možnost »Dovoli IP videa«.</span><span class="sxs-lookup"><span data-stu-id="d83fd-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="d83fd-114">Nato dodelite pravilnik uporabnikom.</span><span class="sxs-lookup"><span data-stu-id="d83fd-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="d83fd-115">**Dodelitev pravilnika o srečanju uporabnikom**</span><span class="sxs-lookup"><span data-stu-id="d83fd-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="d83fd-116">V levem podoknu za krmarjenje Skrbniškega središča za Microsoft Teams pojdite v razdelek **Uporabniki** in kliknite uporabnika.</span><span class="sxs-lookup"><span data-stu-id="d83fd-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="d83fd-117">Izberite uporabnika tako, da kliknete levo stran imena uporabnika, nato pa kliknite **Uredi nastavitve**.</span><span class="sxs-lookup"><span data-stu-id="d83fd-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="d83fd-118">V **razdelku Pravilnik** srečanja izberite pravilnik, ki ga želite dodeliti, in nato kliknite **Uporabi.**</span><span class="sxs-lookup"><span data-stu-id="d83fd-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="d83fd-119">Če želite več informacij, glejte [Upravljanje pravilnikov za srečanja v teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="d83fd-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
