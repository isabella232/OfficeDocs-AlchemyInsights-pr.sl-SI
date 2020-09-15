---
title: 'Napaka: pravila v tem računalniku se ne ujemajo'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690979"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="019c7-102">Napaka: pravila v tem računalniku se ne ujemajo</span><span class="sxs-lookup"><span data-stu-id="019c7-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="019c7-103">Če si želite ogledati posodobljene stanje te znane težave, si oglejte [pravila v tem računalniku se ne ujemajo s pravili v Microsoft Exchangeu](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="019c7-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="019c7-104">Outlookova skupina je izvedla popravek v gradnji 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="019c7-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="019c7-105">Popravek je že na ravni Insider Fast in bo na mesečni kanal konec junija 2020.</span><span class="sxs-lookup"><span data-stu-id="019c7-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="019c7-106">Ko imate nespremenljivo graditev, se lahko prikaže poziv» katera pravila želite ohraniti «še zadnjič.</span><span class="sxs-lookup"><span data-stu-id="019c7-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="019c7-107">Izberite strežnik, ko ste pozvani, nato pa se vrnite v Outlook in znova omogočite vsa pravila, ki so bila onemogočena.</span><span class="sxs-lookup"><span data-stu-id="019c7-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="019c7-108">Preden je popravek na voljo, uporabite to nadomestno rešitev:</span><span class="sxs-lookup"><span data-stu-id="019c7-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="019c7-109">Nadomestna **rešitev**: v nedavnih poročilih je prišlo do težave za tiste, ki so ustvarile le pravila odjemalca v namizni različici Outlooka.</span><span class="sxs-lookup"><span data-stu-id="019c7-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="019c7-110">Če še vedno prihaja do težave, razmislite o brisanju pravil in nato ustvarite in urejajte pravila le v programu OWA (Outlook Web App), dokler težava ni odpravljena.</span><span class="sxs-lookup"><span data-stu-id="019c7-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="019c7-111">Če pravil ne morete izbrisati ročno, lahko zaženete Outlookov ukaz, ko zaženete Outlook tako, da zaženete Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="019c7-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="019c7-112">Tako boste izbrisali pravila odjemalec in strežnik.</span><span class="sxs-lookup"><span data-stu-id="019c7-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="019c7-113">Izbrisala bo vsa pravila za vse račune v Outlookovem profilu.</span><span class="sxs-lookup"><span data-stu-id="019c7-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="019c7-114">Ta ukaz je nadalje dokumentiran v članku stikala ukazne vrstice.</span><span class="sxs-lookup"><span data-stu-id="019c7-114">This command is further documented in the Command-line switches article.</span></span>

