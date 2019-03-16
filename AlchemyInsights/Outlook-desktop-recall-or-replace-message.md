---
title: Razgled pult odpoklic ali Zamenjaj e-pošto
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657059"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="6a02f-102">Preklic ali zamenjava e-pošto</span><span class="sxs-lookup"><span data-stu-id="6a02f-102">Recall or replace an email message</span></span>

- <span data-ttu-id="6a02f-103">Kot admin, lahko **odpoklic sporočila v imenu uporabnik using PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="6a02f-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="6a02f-104">Sporočila iz centra za admin ne more spomniti.</span><span class="sxs-lookup"><span data-stu-id="6a02f-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="6a02f-105">Lahko **samo Preklic sporočila, ki so poslana ljudem v organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="6a02f-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="6a02f-106">Če je bilo sporočilo poslano na Gmail naslov, na primer, lahko ne spomnim to.</span><span class="sxs-lookup"><span data-stu-id="6a02f-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="6a02f-107">Lahko **samo Preklic sporočila, poslana iz Outlook 2016 na PC**.</span><span class="sxs-lookup"><span data-stu-id="6a02f-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="6a02f-108">Če uporabnik pošlje sporočilo z uporabo Outlook za Mac ali Outlook v spletu, lahko spomnim.</span><span class="sxs-lookup"><span data-stu-id="6a02f-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="6a02f-109">Preklicu ali zamenjavi e-pošto:</span><span class="sxs-lookup"><span data-stu-id="6a02f-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="6a02f-110">V podoknu z mapami na levi strani Outlookovega okna, izberite mapo Poslano.</span><span class="sxs-lookup"><span data-stu-id="6a02f-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="6a02f-111">Dvokliknite sporočilo, da želite preklicati razkleniti to.</span><span class="sxs-lookup"><span data-stu-id="6a02f-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="6a02f-112">Izberite **sporočilo** , in nato izberite **dejanja** > **Opozoriti na to sporočilo**.</span><span class="sxs-lookup"><span data-stu-id="6a02f-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="6a02f-113">Izberite **izbrisati neprebrane kopije tega sporočila** ali **izbrisati neprebrane kopije in zamenjati z novim sporočilom**in izberite **OK**.</span><span class="sxs-lookup"><span data-stu-id="6a02f-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="6a02f-114">Če pošiljate sporočilo zamenjavo, sestaviti sporočilo in izberite **Pošlji**.</span><span class="sxs-lookup"><span data-stu-id="6a02f-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="6a02f-115">Uspeh ali neuspeh Preklic sporočila je odvisna od prejemnika nastavitve v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="6a02f-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="6a02f-116">Koraki za preverjanje na odpoklic, glejte [Ta članek](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="6a02f-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="6a02f-117">Iskanje in brisanje e-poštnih sporočil v vaši organizaciji</span><span class="sxs-lookup"><span data-stu-id="6a02f-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="6a02f-118">Če niste svetovnih admin, mora vaš račun dodan eDiscovery vlogo upravitelja ali skladnost iskanje upravljalne vloge za iskanje sporočil.</span><span class="sxs-lookup"><span data-stu-id="6a02f-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="6a02f-119">Èe ¾elite zbrisati sporoèila, boste morali pridružiti skupine vlog »Upravljanje organizacije «ali iskanje in Počisti upravljalne vloge.</span><span class="sxs-lookup"><span data-stu-id="6a02f-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="6a02f-120">Dovoljenja za te vloge so dodeljeni v [center za varnost in skladnost](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="6a02f-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="6a02f-121">[Ustvari vsebino iskanje](https://docs.microsoft.com/office365/securitycompliance/content-search) najti sporočilo za brisanje.</span><span class="sxs-lookup"><span data-stu-id="6a02f-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="6a02f-122">[Povezati varnost in skladnost Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="6a02f-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="6a02f-123">Če uporabljate preverjanje pristnosti multifaktorske, glejte [povezovanje Office 365 varnost in skladnost Center PowerShell uporablja preverjanje pristnosti multifaktorske](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="6a02f-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>