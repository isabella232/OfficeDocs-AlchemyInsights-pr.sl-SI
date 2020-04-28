---
title: Dodajanje zunanjih uporabnikov v distribucijsko skupino
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910948"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="72287-102">Dodajanje zunanjih uporabnikov v distribucijsko skupino</span><span class="sxs-lookup"><span data-stu-id="72287-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="72287-103">Dodajanje zunanjega stika distribucijski skupini (DG) je postopek v dveh korakih:</span><span class="sxs-lookup"><span data-stu-id="72287-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="72287-104">Ustvarite e-poštni stik za zunanjega uporabnika:</span><span class="sxs-lookup"><span data-stu-id="72287-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="72287-105">V skrbniškem središču pojdite na stran» **Users** > [stiki](https://admin.microsoft.com/adminportal/home#/Contact) uporabnikov «.</span><span class="sxs-lookup"><span data-stu-id="72287-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="72287-106">Izberite **Dodaj vizitko**.</span><span class="sxs-lookup"><span data-stu-id="72287-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="72287-107">Vnesite informacije za stik in izberite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="72287-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="72287-108">Dodajanje e-poštnega stika v svoj GD:</span><span class="sxs-lookup"><span data-stu-id="72287-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="72287-109">V skrbniškem središču pojdite[na stran](https://admin.microsoft.com/adminportal/home#/groups) skupine **skupin** > .</span><span class="sxs-lookup"><span data-stu-id="72287-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="72287-110">Poiščite GD, ki ga želite dodati zunanjemu uporabniku, in ga izberite, da odprete pogovorno okno za urejanje.</span><span class="sxs-lookup"><span data-stu-id="72287-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="72287-111">Na zavihku» **člani** «izberite **Prikaži vse in upravljajte člane**.</span><span class="sxs-lookup"><span data-stu-id="72287-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="72287-112">Izberite **Dodaj člane**.</span><span class="sxs-lookup"><span data-stu-id="72287-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="72287-113">Izberite e-poštni stik, ki ste ga ustvarili v prejšnjem koraku, in nato izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="72287-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="72287-114">Če po tem postopku zunanji uporabniki ne morejo pošiljati e-poštnih sporočil generalnemu direktoratu ali ne prejemajo e-poštnih sporočil, je lahko to, da je GD označen samo za omogočanje e-poštnih sporočil od notranjih uporabnikov.</span><span class="sxs-lookup"><span data-stu-id="72287-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="72287-115">To konfiguracijo lahko preverite in odpravite po navodilih [tukaj](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="72287-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="72287-116">**Opomba:** Ta navodila ne veljajo, če je vrsta skupine» skupina Microsoft 365 «namesto» skupina prejemnikov «.</span><span class="sxs-lookup"><span data-stu-id="72287-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="72287-117">V tem primeru lahko zunanjega uporabnika dodate neposredno v skupino iz Outlooka.</span><span class="sxs-lookup"><span data-stu-id="72287-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="72287-118">Podrobne informacije o Microsoftovih 365 skupinah gostov, kot tudi navodila za dodajanje zunanjih gostov, je mogoče najti v [tem članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="72287-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  