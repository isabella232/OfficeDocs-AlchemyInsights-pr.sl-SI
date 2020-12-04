---
title: Dodajanje ali odstranjevanje pooblaščenca v Outlooku za Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573812"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="e051d-102">Dodajanje ali odstranjevanje pooblaščenca v Outlooku za Windows</span><span class="sxs-lookup"><span data-stu-id="e051d-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="e051d-103">Če želite dodati pooblaščenca v Outlooku za Windows:</span><span class="sxs-lookup"><span data-stu-id="e051d-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="e051d-104">Kliknite zavihek **Datoteka** , ki mu sledi **nastavitev računa**, nato pa izberite **pooblaščen dostop**.</span><span class="sxs-lookup"><span data-stu-id="e051d-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="e051d-105">Kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="e051d-105">Click on **Add**.</span></span> <span data-ttu-id="e051d-106">Če se **Dodajanje** ne prikaže, aktivna povezava morda ne obstaja med Outlookom in storitvijo Exchange.</span><span class="sxs-lookup"><span data-stu-id="e051d-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="e051d-107">V Outlookovi vrstici stanja je prikazano stanje povezave.</span><span class="sxs-lookup"><span data-stu-id="e051d-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="e051d-108">Vnesite ime osebe, ki jo želite imenovati kot pooblaščenca, ali pa poiščite in izberite ime na seznamu rezultatov iskanja.</span><span class="sxs-lookup"><span data-stu-id="e051d-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e051d-109">Pooblaščenec mora biti oseba na globalnem seznamu naslovov v organizaciji Exchange (GAL).</span><span class="sxs-lookup"><span data-stu-id="e051d-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="e051d-110">Kliknite» **Dodaj** «in nato» **v redu «**.</span><span class="sxs-lookup"><span data-stu-id="e051d-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="e051d-111">V pogovornem oknu **pooblaščena dovoljenja** sprejmite privzete nastavitve dovoljenj ali izberite ravni dostopa po meri za Exchangeeve mape.</span><span class="sxs-lookup"><span data-stu-id="e051d-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="e051d-112">Če pooblaščenec potrebuje dovoljenje za delo le z povabili na srečanje in odgovori, so privzete nastavitve dovoljenj, kot je **pooblaščenec, prejele kopije sporočil, povezanih z srečanjem, ki so poslana meni** , zadoščajo.</span><span class="sxs-lookup"><span data-stu-id="e051d-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="e051d-113">Nastavitev dovoljenja za **mapo» Prejeto «** lahko pustite **brez**.</span><span class="sxs-lookup"><span data-stu-id="e051d-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="e051d-114">Povabila na srečanje in odgovori se bodo odpravili neposredno v mapo» Prejeto «pooblaščenca.</span><span class="sxs-lookup"><span data-stu-id="e051d-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e051d-115">Pooblaščenec je privzeto dodeljen **urejevalniku (lahko bere, ustvarja in spreminja elemente)** dovoljenje za mapo **koledar** .</span><span class="sxs-lookup"><span data-stu-id="e051d-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="e051d-116">Ko pooblaščenec odgovori na srečanje v vašem imenu, se ta samodejno doda v mapo s **koledarjem** .</span><span class="sxs-lookup"><span data-stu-id="e051d-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="e051d-117">Če želite poslati sporočilo, da obvesti pooblaščenca o spremenjenih dovoljenjih, potrdite potrditveno polje **samodejno Pošlji sporočilo, da je pooblaščeno povzemanje teh dovoljenj** .</span><span class="sxs-lookup"><span data-stu-id="e051d-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="e051d-118">Če želite, potrdite potrditveno polje **Pooblaščenec lahko vidi moje zasebne elemente** .</span><span class="sxs-lookup"><span data-stu-id="e051d-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="e051d-119">Ta nastavitev vpliva na vse Exchangeeve mape.</span><span class="sxs-lookup"><span data-stu-id="e051d-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="e051d-120">To vključuje vsa sporočila, stike, koledar, opravila, zapiske in mape dnevnika.</span><span class="sxs-lookup"><span data-stu-id="e051d-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="e051d-121">Dostop do zasebnih elementov ni mogoče dodeliti le v določenih mapah.</span><span class="sxs-lookup"><span data-stu-id="e051d-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="e051d-122">Izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="e051d-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="e051d-123">Sporočila, poslana z dovoljenjem» Pošlji v imenu «, vključujejo oba pooblaščenca in vaša imena zraven možnosti **od**.</span><span class="sxs-lookup"><span data-stu-id="e051d-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="e051d-124">Ko je sporočilo poslano z dovoljenjem» Pošlji kot «, se prikaže le vaše ime.</span><span class="sxs-lookup"><span data-stu-id="e051d-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="e051d-125">Ko dodate osebo kot pooblaščenca, lahko dodate Exchangeev nabiralnik v svoj Outlookov profil.</span><span class="sxs-lookup"><span data-stu-id="e051d-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="e051d-126">Če želite navodila, glejte [upravljanje elementov pošte in koledarja druge osebe](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="e051d-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="e051d-127">Če želite odstraniti pooblaščenca v Outlooku za Windows:</span><span class="sxs-lookup"><span data-stu-id="e051d-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="e051d-128">Kliknite zavihek **Datoteka** .</span><span class="sxs-lookup"><span data-stu-id="e051d-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="e051d-129">Kliknite **Nastavitve računa** , ki mu sledi **pooblaščen dostop**.</span><span class="sxs-lookup"><span data-stu-id="e051d-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="e051d-130">Izberite ime pooblaščenca, za katerega želite spremeniti dovoljenja, in nato kliknite **Odstrani** , ki ji sledi» **v redu «**.</span><span class="sxs-lookup"><span data-stu-id="e051d-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
