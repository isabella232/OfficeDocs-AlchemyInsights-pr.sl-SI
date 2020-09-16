---
title: Teams dovoljujejo ali onemogočijo IP video
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670200"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="ade44-102">Teams dovoljujejo ali onemogočijo IP video</span><span class="sxs-lookup"><span data-stu-id="ade44-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="ade44-103">**Spreminjanje ali ustvarjanje pravilnika za srečanje**</span><span class="sxs-lookup"><span data-stu-id="ade44-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="ade44-104">Če želite spremeniti ali ustvariti pravilnik za srečanje, pojdite v **skrbniško središče za Microsoft teams > srečanja > pravilniki o srečanju**.</span><span class="sxs-lookup"><span data-stu-id="ade44-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="ade44-105">Na seznamu izberite pravilnik ali kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="ade44-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="ade44-106">Če ustvarjate nov pravilnik, dodajte ime in opis.</span><span class="sxs-lookup"><span data-stu-id="ade44-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="ade44-107">V imenu ne sme biti posebnih znakov, ime pa ne sme biti daljše od 64 znakov.</span><span class="sxs-lookup"><span data-stu-id="ade44-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="ade44-108">Izberite nastavitve in kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="ade44-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="ade44-109">Recimo, da imate veliko uporabnikov in želite omejiti količino pasovne širine, ki bi jih zahtevala njihova seja.</span><span class="sxs-lookup"><span data-stu-id="ade44-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="ade44-110">Ustvarite nov pravilnik po meri, imenovan »Omejena pasovna širina« in onemogočite te nastavitve:</span><span class="sxs-lookup"><span data-stu-id="ade44-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="ade44-111">V razdelku **Zvok in video**:</span><span class="sxs-lookup"><span data-stu-id="ade44-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="ade44-112">Izklopite možnost »Dovoli snemanje v oblaku«.</span><span class="sxs-lookup"><span data-stu-id="ade44-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="ade44-113">Izklopite možnost »Dovoli IP videa«.</span><span class="sxs-lookup"><span data-stu-id="ade44-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="ade44-114">Nato dodelite pravilnik uporabnikom.</span><span class="sxs-lookup"><span data-stu-id="ade44-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="ade44-115">**Dodelitev pravilnika o srečanju uporabnikom**</span><span class="sxs-lookup"><span data-stu-id="ade44-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="ade44-116">V levem podoknu za krmarjenje Skrbniškega središča za Microsoft Teams pojdite v razdelek **Uporabniki** in kliknite uporabnika.</span><span class="sxs-lookup"><span data-stu-id="ade44-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="ade44-117">Izberite uporabnika tako, da kliknete levo stran imena uporabnika, nato pa kliknite **Uredi nastavitve**.</span><span class="sxs-lookup"><span data-stu-id="ade44-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="ade44-118">V razdelku **pravilnik za srečanje**izberite pravilnik, ki ga želite dodeliti, in nato kliknite **uporabi**.</span><span class="sxs-lookup"><span data-stu-id="ade44-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="ade44-119">Če želite več informacij, glejte [upravljanje pravilnikov za srečanje v aplikaciji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ade44-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
