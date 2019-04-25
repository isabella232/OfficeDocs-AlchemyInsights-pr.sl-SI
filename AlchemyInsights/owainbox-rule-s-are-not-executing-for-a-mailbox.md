---
title: 1332 OWA - Prejeto pravilo(-a) ne izvajate za nabiralnik
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372576"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="d54b9-102">Pravilo za prejeto pošto ne delujejo po pričakovanjih</span><span class="sxs-lookup"><span data-stu-id="d54b9-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="d54b9-103">Preveriti te nastavitve:</span><span class="sxs-lookup"><span data-stu-id="d54b9-103">Verify the following settings:</span></span>

- <span data-ttu-id="d54b9-104">Sporočilo lahko preusmerjeni, posredovana ali odgovorjena samodejno glede na pravila za prejeto pošto le enkrat.</span><span class="sxs-lookup"><span data-stu-id="d54b9-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="d54b9-105">Preusmerjanje pravilo (Prejeto pravilo ali pretok pravilo za pošto, znan tudi kot pravila prenosa) lahko dodate največ deset posredovanje prejemnikov sporočila.</span><span class="sxs-lookup"><span data-stu-id="d54b9-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="d54b9-106">Če želite več informacij, glejte [listu, prevoz, in Prejeto pravilo omejuje](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="d54b9-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="d54b9-107">Pravila za prejeto pošto ne delujejo na nabiralnik nadomestni dnevnika.</span><span class="sxs-lookup"><span data-stu-id="d54b9-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="d54b9-108">Če želite več informacij o dnevniški nadomestne nabiralnik, glejte [nabiralnik dnevnika namestnika](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="d54b9-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="d54b9-109">Če želite odpraviti te težave, glejte [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="d54b9-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="d54b9-110">Če predhodni vprašanji ne uporablja, Prejeto pravilo diagnostičnih poročilo zagnati stopnjujejo izdajo Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="d54b9-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="d54b9-111">Odprite nabiralnik v Outlooku na spletu, in kliknite **Nastavitve** \> **možnosti** \> **Organiziraj e-pošto** \> **pravila za prejeto pošto**.</span><span class="sxs-lookup"><span data-stu-id="d54b9-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="d54b9-112">Na dnu strani kliknite **Če pravil ne delajo kliknite, če želite ustvariti poročilo, diagnostiko**.</span><span class="sxs-lookup"><span data-stu-id="d54b9-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
