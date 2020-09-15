---
title: Outlook Desktop Prekliči ali Zamenjaj e-poštno sporočilo
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664006"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="04961-102">Preklic ali zamenjava Outlookovega e-poštnega sporočila</span><span class="sxs-lookup"><span data-stu-id="04961-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="04961-103">Kot skrbnik lahko v **imenu uporabnikov, ki uporabljajo PowerShell**, prekličete sporočila.</span><span class="sxs-lookup"><span data-stu-id="04961-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="04961-104">Ne morete se spomniti sporočil v skrbniškem središču.</span><span class="sxs-lookup"><span data-stu-id="04961-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="04961-105">**Sporočila, ki so poslana osebam v organizaciji, lahko odpokličete le**.</span><span class="sxs-lookup"><span data-stu-id="04961-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="04961-106">Če je bilo sporočilo poslano na naslov Gmail, ga na primer ne morete preklicati.</span><span class="sxs-lookup"><span data-stu-id="04961-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="04961-107">Sporočila, **poslana iz programa Outlook 2016**, lahko prekličete le v računalniku s sistemom Windows.</span><span class="sxs-lookup"><span data-stu-id="04961-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="04961-108">Če uporabnik pošlje sporočilo z Outlookom za Mac ali Outlookom v spletu, ga ne morete preklicati.</span><span class="sxs-lookup"><span data-stu-id="04961-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="04961-109">Če želite preklicati ali zamenjati e-poštno sporočilo:</span><span class="sxs-lookup"><span data-stu-id="04961-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="04961-110">V podoknu» mapa «na levi strani Outlookovega okna izberite mapo Poslano.</span><span class="sxs-lookup"><span data-stu-id="04961-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="04961-111">Dvokliknite sporočilo, ki ga želite preklicati, da ga odprete.</span><span class="sxs-lookup"><span data-stu-id="04961-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="04961-112">Izberite zavihek **sporočilo** , nato pa izberite **dejanja**  >  **Prekliči to sporočilo**.</span><span class="sxs-lookup"><span data-stu-id="04961-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="04961-113">Izberite **Izbriši neprebrane kopije tega sporočila** ali **Izbriši neprebrane kopije in jih Zamenjaj z novim sporočilom**, nato pa izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="04961-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="04961-114">Če pošiljate nadomestno sporočilo, sestavite sporočilo in nato izberite **Pošlji**.</span><span class="sxs-lookup"><span data-stu-id="04961-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="04961-115">Uspeh ali neuspeh odpoklica sporočil je odvisen od nastavitev prejemnika v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="04961-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="04961-116">Če želite navodila za preverjanje odpoklica, glejte [Ta članek](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="04961-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="04961-117">Iskanje in brisanje e-poštnih sporočil v organizaciji</span><span class="sxs-lookup"><span data-stu-id="04961-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="04961-118">Če niste globalni skrbnik, mora biti vaš račun dodan v vlogo upravitelja E-odkrivanje ali upravljanje iskanja skladnosti, če želite poiskati sporočila.</span><span class="sxs-lookup"><span data-stu-id="04961-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="04961-119">Če želite izbrisati sporočila, se morate vključiti v skupino vlog za upravljanje organizacije ali vlogo za upravljanje iskanja in čiščenja.</span><span class="sxs-lookup"><span data-stu-id="04961-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="04961-120">Dovoljenja za te vloge so dodeljena v [središču za varnost in skladnost s predpisi](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="04961-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="04961-121">[Ustvarite iskanje vsebine](https://docs.microsoft.com/microsoft-365/compliance/content-search) , da poiščete sporočilo, ki ga želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="04961-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="04961-122">[Povežite se s središčem PowerShell za varnost in skladnost s predpisi](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="04961-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="04961-123">Če uporabljate več dejavnikov preverjanja pristnosti, si oglejte [povezovanje z lupino za varnost in skladnost s programom Microsoft 365 z uporabo več dejavnikov preverjanja pristnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="04961-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>