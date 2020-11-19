---
title: Preklic ali zamenjava e-poštnega sporočila
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353522"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="09418-102">Preklic ali zamenjava e-poštnega sporočila v programu Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="09418-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="09418-103">**Sporočila, ki so poslana osebam v organizaciji, lahko odpokličete le**.</span><span class="sxs-lookup"><span data-stu-id="09418-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="09418-104">Če je bilo na primer sporočilo poslano v naslov Gmail, ga ne morete preklicati.</span><span class="sxs-lookup"><span data-stu-id="09418-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="09418-105">Prekličete lahko **le sporočila, poslana iz Outlooka za računalnik s** sistemom Windows.</span><span class="sxs-lookup"><span data-stu-id="09418-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="09418-106">Če uporabnik pošlje sporočilo z Outlookom za Mac ali Outlookom v spletu, ga ne morete preklicati.</span><span class="sxs-lookup"><span data-stu-id="09418-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="09418-107">Kot skrbnik najemnika lahko v imenu uporabnikov prekličete sporočila, in **sicer tako, da uporabite PowerShell** (če želite več informacij, glejte: [iskanje in brisanje e-poštnih sporočil](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="09418-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="09418-108">Ne morete se spomniti sporočil v skrbniškem središču.</span><span class="sxs-lookup"><span data-stu-id="09418-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="09418-109">Če želite več informacij, se pomaknite navzdol do možnosti» iskanje in brisanje e-poštnih sporočil v organizaciji «.</span><span class="sxs-lookup"><span data-stu-id="09418-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="09418-110">**Preklic ali zamenjava poslanega e-poštnega sporočila**</span><span class="sxs-lookup"><span data-stu-id="09418-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="09418-111">V podoknu» mapa «na levi strani Outlookovega okna izberite mapo Poslano.</span><span class="sxs-lookup"><span data-stu-id="09418-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="09418-112">Odprite sporočilo, ki ga želite preklicati.</span><span class="sxs-lookup"><span data-stu-id="09418-112">Open the message that you want to recall.</span></span> <span data-ttu-id="09418-113">Če želite odpreti sporočilo, morate dvoklikniti.</span><span class="sxs-lookup"><span data-stu-id="09418-113">You must double-click to open the message.</span></span> <span data-ttu-id="09418-114">Če izberete sporočilo, da se prikaže v podoknu za branje, ne boste mogli preklicati sporočila.</span><span class="sxs-lookup"><span data-stu-id="09418-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="09418-115">Na zavihku sporočilo izberite **dejanja**  >  **Prekliči to sporočilo**.</span><span class="sxs-lookup"><span data-stu-id="09418-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="09418-116">Izberite **Izbriši neprebrane kopije tega sporočila** ali **Izbriši neprebrane kopije in jih Zamenjaj z novim sporočilom**, nato pa izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="09418-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="09418-117">Če pošiljate nadomestno sporočilo, sestavite sporočilo in izberite **Pošlji**.</span><span class="sxs-lookup"><span data-stu-id="09418-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="09418-118">Uspeh ali neuspeh odpoklica sporočila je odvisen od nastavitev prejemnikov v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="09418-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="09418-119">Če želite več informacij, vključno s tem, kako preverite preklic, glejte [preklic ali zamenjava e-poštnega sporočila, ki ste ga poslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="09418-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="09418-120">Če **_želite poiskati in izbrisati e-poštna sporočila v vaši organizaciji_**, je najlažje, če ste globalni skrbnik. Če niste globalni skrbnik, mora biti vaš račun dodan v skupino vlog E-odkrivanje Manager ali pa na vlogo za upravljanje iskanja skladnosti.</span><span class="sxs-lookup"><span data-stu-id="09418-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="09418-121">Če želite izbrisati sporočila, se morate vključiti v skupino vlog za upravljanje organizacije ali vlogo za upravljanje iskanja in čiščenja.</span><span class="sxs-lookup"><span data-stu-id="09418-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="09418-122">Dovoljenja za te vloge so dodeljena v [središču za skladnost varnostnega &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="09418-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="09418-123">[Ustvarite iskanje vsebine](https://docs.microsoft.com/microsoft-365/compliance/content-search) , da poiščete sporočilo, ki ga želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="09418-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="09418-124">[Vzpostavi povezavo z varnostnim središčem v središču za skladnost z varnostjo &](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="09418-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="09418-125">Če uporabljate MFA (multi-Factor Authentication), si oglejte [povezovanje s storitvijo Microsoft 365 Security & skladnost s centrom PowerShell z več faktorji preverjanja pristnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="09418-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
