---
title: Dodajanje zunanjih uporabnikov v distribucijsko skupino
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737889"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="da057-102">Dodajanje zunanjih uporabnikov v distribucijsko skupino</span><span class="sxs-lookup"><span data-stu-id="da057-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="da057-103">Dodajanje zunanjega stika distribucijski skupini (DG) je postopek v dveh korakih:</span><span class="sxs-lookup"><span data-stu-id="da057-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="da057-104">Ustvarite e-poštni stik za zunanjega uporabnika:</span><span class="sxs-lookup"><span data-stu-id="da057-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="da057-105">V skrbniškem središču pojdite na stran» \*\*\*\* > [stiki](https://admin.microsoft.com/adminportal/home#/Contact) uporabnikov «.</span><span class="sxs-lookup"><span data-stu-id="da057-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="da057-106">Izberite **Dodaj vizitko**.</span><span class="sxs-lookup"><span data-stu-id="da057-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="da057-107">Vnesite informacije za stik in izberite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="da057-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="da057-108">Dodajanje e-poštnega stika v svoj GD:</span><span class="sxs-lookup"><span data-stu-id="da057-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="da057-109">V skrbniškem središču pojdite[na stran](https://admin.microsoft.com/adminportal/home#/groups) skupine **skupin** > .</span><span class="sxs-lookup"><span data-stu-id="da057-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="da057-110">Poiščite GD, ki ga želite dodati zunanjemu uporabniku, in ga izberite, da odprete pogovorno okno za urejanje.</span><span class="sxs-lookup"><span data-stu-id="da057-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="da057-111">Na zavihku» **člani** «izberite **Prikaži vse in upravljajte člane**.</span><span class="sxs-lookup"><span data-stu-id="da057-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="da057-112">Izberite **Dodaj člane**.</span><span class="sxs-lookup"><span data-stu-id="da057-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="da057-113">Izberite e-poštni stik, ki ste ga ustvarili v prejšnjem koraku, in nato izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="da057-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="da057-114">Če po tem postopku zunanji uporabniki ne morejo pošiljati e-poštnih sporočil generalnemu direktoratu ali ne prejemajo e-poštnih sporočil, je lahko to, da je GD označen samo za omogočanje e-poštnih sporočil od notranjih uporabnikov.</span><span class="sxs-lookup"><span data-stu-id="da057-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="da057-115">To konfiguracijo lahko preverite in odpravite po navodilih [tukaj](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="da057-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="da057-116">**Opomba:** Ta navodila ne veljajo, če je vrsta skupine» skupina Office 365 «namesto» skupina prejemnikov «.</span><span class="sxs-lookup"><span data-stu-id="da057-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="da057-117">V tem primeru lahko zunanjega uporabnika dodate neposredno v skupino iz Outlooka.</span><span class="sxs-lookup"><span data-stu-id="da057-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="da057-118">Podrobne informacije o skupini Office 365 in navodila za dodajanje zunanjih gostov so na voljo v [tem članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="da057-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  