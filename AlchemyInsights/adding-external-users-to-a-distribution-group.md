---
title: Dodajanje zunanjih uporabnikov v skupino prejemnikov
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663529"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="acec8-102">Dodajanje zunanjih uporabnikov v skupino prejemnikov</span><span class="sxs-lookup"><span data-stu-id="acec8-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="acec8-103">Dodajanje zunanjega stika v skupino prejemnikov (DG) je postopek v dveh korakih:</span><span class="sxs-lookup"><span data-stu-id="acec8-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="acec8-104">Ustvarjanje poštnega stika za zunanjega uporabnika:</span><span class="sxs-lookup"><span data-stu-id="acec8-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="acec8-105">V skrbniškem središču pojdite na **Users**  >  stran[stiki](https://admin.microsoft.com/adminportal/home#/Contact) z uporabniki.</span><span class="sxs-lookup"><span data-stu-id="acec8-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="acec8-106">Izberite **Dodaj stik**.</span><span class="sxs-lookup"><span data-stu-id="acec8-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="acec8-107">Vnesite podatke za stik in izberite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="acec8-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="acec8-108">Dodajte poštni stik v GD:</span><span class="sxs-lookup"><span data-stu-id="acec8-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="acec8-109">V skrbniškem središču pojdite na stran skupine **skupin**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="acec8-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="acec8-110">Poiščite generalnega direktorata, ki ga želite dodati zunanjemu uporabniku, in ga izberite, da odprete pogovorno okno za urejanje.</span><span class="sxs-lookup"><span data-stu-id="acec8-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="acec8-111">Na zavihku **člani** izberite **Ogled vseh in upravljanje članov**.</span><span class="sxs-lookup"><span data-stu-id="acec8-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="acec8-112">Izberite **Dodaj člane**.</span><span class="sxs-lookup"><span data-stu-id="acec8-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="acec8-113">Izberite poštni stik, ki ste ga ustvarili v prejšnjem koraku, in nato izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="acec8-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="acec8-114">Če po teh navodilih zunanji uporabniki ne morejo poslati e-poštnih sporočil generalnemu direktoratu ali pa ne prejemajo e-poštnih sporočil, je to lahko, da je GD označen le za e-poštna sporočila internih uporabnikov.</span><span class="sxs-lookup"><span data-stu-id="acec8-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="acec8-115">To konfiguracijo lahko preverite in jo odpravite tako, da upoštevate navodila [tukaj](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="acec8-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="acec8-116">**Opomba:** Ta navodila ne veljajo, če je vrsta skupine» skupina Microsoft 365 «namesto» skupina prejemnikov «.</span><span class="sxs-lookup"><span data-stu-id="acec8-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="acec8-117">Če je to res, lahko zunanjega uporabnika dodate neposredno v skupino iz Outlooka.</span><span class="sxs-lookup"><span data-stu-id="acec8-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="acec8-118">V [tem članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)so na voljo podrobne informacije o skupinah v storitvi Microsoft 365, kot tudi navodila za dodajanje zunanjih gostov.</span><span class="sxs-lookup"><span data-stu-id="acec8-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  