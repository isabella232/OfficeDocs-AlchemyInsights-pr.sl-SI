---
title: 'Napaka: Pravila v tem računalniku se ne ujemajo'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782968"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="3e83f-102">Napaka: Pravila v tem računalniku se ne ujemajo</span><span class="sxs-lookup"><span data-stu-id="3e83f-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="3e83f-103">Če želite videti posodobljeno stanje te znane težave, glejte Pravila v tem računalniku se ne ujemajo [s pravili v Microsoft Exchangeu.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="3e83f-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="3e83f-104">Skupina za Outlook je v gradili 12928.10000 izvedla popravek.</span><span class="sxs-lookup"><span data-stu-id="3e83f-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="3e83f-105">Popravek je že na voljo v programu Insider Fast in bo v drugi juniju 2020 na voljo za mesečni kanal.</span><span class="sxs-lookup"><span data-stu-id="3e83f-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="3e83f-106">Ko imate popravljeno gradnjo, se lahko znova prikaže poziv »Katera pravila želite obdržati«.</span><span class="sxs-lookup"><span data-stu-id="3e83f-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="3e83f-107">Ko ste pozvani, izberite Strežnik, nato pa se v Outlooku znova vženite in znova omogočite vsa onemogočena pravila.</span><span class="sxs-lookup"><span data-stu-id="3e83f-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="3e83f-108">Dokler popravek ni na voljo, uporabite to rešitev:</span><span class="sxs-lookup"><span data-stu-id="3e83f-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="3e83f-109">**Rešitev: V** nedavnih poročilih je prišlo do težave pri osebah, ki so le ustvarila pravila odjemalca v namizni različici Outlooka.</span><span class="sxs-lookup"><span data-stu-id="3e83f-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="3e83f-110">Če težave ne morete odpraviti, premislite o brisanju pravil in nato ustvarite in uredite pravila le v programu OWA (Outlook Web App), dokler težava ne bo odpravljena.</span><span class="sxs-lookup"><span data-stu-id="3e83f-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="3e83f-111">Če pravil ne morete izbrisati ročno, lahko zaženete Outlookov ukaz, ko zaženete Outlook tako, da zaženete Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="3e83f-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="3e83f-112">S tem izbrišete pravila odjemalca in strežnika.</span><span class="sxs-lookup"><span data-stu-id="3e83f-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="3e83f-113">Izbrisala bo vsa pravila za vse račune v Outlookovem profilu.</span><span class="sxs-lookup"><span data-stu-id="3e83f-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="3e83f-114">Ta ukaz je podrobneje zabeležen v članku Stikala ukazne vrstice.</span><span class="sxs-lookup"><span data-stu-id="3e83f-114">This command is further documented in the Command-line switches article.</span></span>

