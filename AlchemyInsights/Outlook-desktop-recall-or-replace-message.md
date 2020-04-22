---
title: Outlook Desktop se spomni ali zamenja e-poštno sporočilo
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687526"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="e2fb5-102">Odpoklic ali zamenjava Outlookovega e-poštnega sporočila</span><span class="sxs-lookup"><span data-stu-id="e2fb5-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="e2fb5-103">Kot admin, lahko **odpoklic sporočil v imenu uporabnikov, ki uporabljajo PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="e2fb5-104">Ne morete se spomniti sporočil iz skrbniškega centra.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="e2fb5-105">Prikličete lahko **samo sporočila, poslana osebam v vaši organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="e2fb5-106">Če je bilo sporočilo poslano v Gmailov naslov, ga na primer ne morete spomniti.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="e2fb5-107">**V računalniku lahko odpokličejo samo sporočila, poslana iz outlooka 2016**.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="e2fb5-108">Če uporabnik pošlje sporočilo z Outlookom za Mac ali Outlook v spletu, ga ne morete spomniti.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="e2fb5-109">Preklic ali zamenjava e-poštnega sporočila:</span><span class="sxs-lookup"><span data-stu-id="e2fb5-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="e2fb5-110">V podoknu map na levi strani Outlookovega okna izberite mapo Poslani predmeti.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="e2fb5-111">Dvokliknite sporočilo, ki ga želite opomniti, da ga odprete.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="e2fb5-112">Izberite zavihek **sporočilo** in nato izberite **dejanja** > , ki se**odpokličejo v to sporočilo**.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="e2fb5-113">Izberite **Izbriši neprebrane kopije tega sporočila** ali **izbrišite neprebrane kopije in zamenjajte novo sporočilo**, nato pa izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="e2fb5-114">Če pošiljate nadomestno sporočilo, sestavite sporočilo in nato izberite **Pošlji**.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="e2fb5-115">Uspeh ali neuspeh odpoklica sporočila je odvisen od prejemnikov nastavitev v programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="e2fb5-116">Če želite preveriti odpoklic, si oglejte [Ta članek](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="e2fb5-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="e2fb5-117">Iskanje in brisanje e-poštnih sporočil v organizaciji</span><span class="sxs-lookup"><span data-stu-id="e2fb5-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="e2fb5-118">Če niste globalni skrbnik, morate račun dodati vlogi upravitelja e-odkrivanja ali vlogi za upravljanje iskanja po skladnosti za iskanje sporočil.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="e2fb5-119">Če želite izbrisati sporočila, se morate pridružiti skupini vlog za upravljanje organizacije ali funkciji za upravljanje iskanja in čiščenja.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="e2fb5-120">Dovoljenja za te vloge so dodeljena v [središču za varnost in skladnost](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="e2fb5-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="e2fb5-121">[Ustvarite iskanje po vsebini](https://docs.microsoft.com/office365/securitycompliance/content-search) in poiščite sporočilo, ki ga želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="e2fb5-122">[Vzpostavite povezavo z lupino za varnostno in skladnost center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="e2fb5-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="e2fb5-123">Če uporabljate večfaktorsko preverjanje pristnosti, glejte [Vzpostavljanje povezave z Microsoft 365 varnostjo in lupino središča za skladnost z uporabo večfaktorskega preverjanja pristnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="e2fb5-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>