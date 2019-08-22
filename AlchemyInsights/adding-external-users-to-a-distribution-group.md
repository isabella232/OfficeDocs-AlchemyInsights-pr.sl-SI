---
title: Zunanje uporabnike dodate skupine prejemnikov
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494543"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="9fd9d-102">Zunanji uporabniki dodati skupine prejemnikov?</span><span class="sxs-lookup"><span data-stu-id="9fd9d-102">Add external users to a Distribution Group?</span></span>

<span data-ttu-id="9fd9d-103">Dodajanje zunanji stik za distribucijo skupine (direktorata) je 2 korakih:</span><span class="sxs-lookup"><span data-stu-id="9fd9d-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="9fd9d-104">Ustvarite poštni stik za zunanjega uporabnika:</span><span class="sxs-lookup"><span data-stu-id="9fd9d-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="9fd9d-105">V skrbniškem središču, iti k **uporabnik** > strani[Kontakt](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="9fd9d-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="9fd9d-106">Izberite **Dodaj stik**.</span><span class="sxs-lookup"><span data-stu-id="9fd9d-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="9fd9d-107">Vnesti podatke za stik in izberite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="9fd9d-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="9fd9d-108">Poštni stik dodate vaš DG:</span><span class="sxs-lookup"><span data-stu-id="9fd9d-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="9fd9d-109">V središču admin, pojdite na **skupine** > [skupine](https://admin.microsoft.com/adminportal/home#/groups) strani.</span><span class="sxs-lookup"><span data-stu-id="9fd9d-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="9fd9d-110">Poišči GD želite dodati zunanji uporabnik, in izberite, da odprete pogovorno okno za urejanje.</span><span class="sxs-lookup"><span data-stu-id="9fd9d-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="9fd9d-111">Na zavihku **»člani«** izberite **vse ogled in upravljanje članov**.</span><span class="sxs-lookup"><span data-stu-id="9fd9d-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="9fd9d-112">Izberite **Dodaj člane**.</span><span class="sxs-lookup"><span data-stu-id="9fd9d-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="9fd9d-113">Izberite poštni stik, ki ste jo ustvarili v prejšnjem koraku, in nato izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="9fd9d-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="9fd9d-114">Če po naslednjim korakom zunanji uporabniki ne more poslati e-pošto GD ali ne prejemajo e-pošto iz njega, lahko, da GD je označen, da dovoljuje le e-pošto iz notranjih uporabnikov.</span><span class="sxs-lookup"><span data-stu-id="9fd9d-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="9fd9d-115">Si lahko ogledate ta konfiguracija in popraviti po navodila [tukaj](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="9fd9d-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="9fd9d-116">**Opomba:** Teh navodil ne uporabljajo, če vaša skupina vrsta "Office 365 skupina" namesto "Distribucijsko skupino."</span><span class="sxs-lookup"><span data-stu-id="9fd9d-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="9fd9d-117">Če je temu tako, lahko dodate zunanjo uporabnik neposredno skupini iz Outlooka.</span><span class="sxs-lookup"><span data-stu-id="9fd9d-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="9fd9d-118">V [tem članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)najdete podrobne informacije o Office 365 skupine gostov, kot tudi navodila za dodajanje zunanje goste.</span><span class="sxs-lookup"><span data-stu-id="9fd9d-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  