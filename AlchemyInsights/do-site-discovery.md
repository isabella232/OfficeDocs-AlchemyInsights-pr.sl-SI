---
title: Do odkrivanja mesta
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694557"
---
# <a name="do-site-discovery"></a><span data-ttu-id="5e76d-102">Do odkrivanja mesta</span><span class="sxs-lookup"><span data-stu-id="5e76d-102">Do site discovery</span></span>

<span data-ttu-id="5e76d-103">Če vaša organizacija še vedno uporablja podedovane spletne programe in načrte za uporabo programa Internet Explorer (ki ga večina strank naredi), naredite nekaj dodatnega odkrivanja mesta.</span><span class="sxs-lookup"><span data-stu-id="5e76d-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="5e76d-104">**Uvedli ste že starejšo različico programa Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="5e76d-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="5e76d-105">Če ste seznam mesta podjetja že konfigurirali tako, da delate za starejšo različico programa Microsoft Edge, je odkrivanje mesta skoraj končano.</span><span class="sxs-lookup"><span data-stu-id="5e76d-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="5e76d-106">Eno stvar, ki jo boste morda morali narediti, je dodajanje nevtralnih mest.</span><span class="sxs-lookup"><span data-stu-id="5e76d-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="5e76d-107">Nevtralna mesta so običajno spletna mesta, ki zagotavljajo enotno prijavo (SSO).</span><span class="sxs-lookup"><span data-stu-id="5e76d-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="5e76d-108">Če se na spletnem mestu Microsoft Edge pogovorite z nevtralnim mestom, potem želite za preverjanje pristnosti ostati v programu Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="5e76d-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="5e76d-109">Če se v načinu Internet Explorerja pogovorite z nevtralnim mestom, lahko v načinu Internet Explorerja ohranite preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="5e76d-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="5e76d-110">Identificirajte katero koli SSO ali druga nevtralna mesta, ki jih uporabljate, in jih dodajte na seznam mesta podjetja.</span><span class="sxs-lookup"><span data-stu-id="5e76d-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="5e76d-111">**Internet Explorer je vaš privzeti brskalnik**</span><span class="sxs-lookup"><span data-stu-id="5e76d-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="5e76d-112">Če uporabljate le Internet Explorer, morda ne veste, katera spletna mesta so nadgradila na sodobne spletne standarde in ki še vedno zahtevajo Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="5e76d-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="5e76d-113">Na seznamu mesta podjetja boste želeli poiskati in dodati ta mesta, da boste lahko uporabljali le način Internet Explorerja le za ta spletna mesta.</span><span class="sxs-lookup"><span data-stu-id="5e76d-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="5e76d-114">[Odkrivanje](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) spletnih mest za podjetja odkrije spletna mesta, ki bi morda potrebovala način Internet Explorerja.</span><span class="sxs-lookup"><span data-stu-id="5e76d-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="5e76d-115">S programom Internet Explorer 11 v sistemu Windows 10, Windows 8,1 ali Windows 7 lahko zbira podatke v računalnikih, v katerih je nameščen Windows Internet Explorer 8.</span><span class="sxs-lookup"><span data-stu-id="5e76d-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="5e76d-116">**Analiziranje podatkov**</span><span class="sxs-lookup"><span data-stu-id="5e76d-116">**Analyze the data**</span></span>

<span data-ttu-id="5e76d-117">Ko zberete podatke o mestu, vam priporočamo, da analizirate podatke s temi štirimi koraki:</span><span class="sxs-lookup"><span data-stu-id="5e76d-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="5e76d-118">Razvrščanje podatkov po domeni in nato prek URL-ja.</span><span class="sxs-lookup"><span data-stu-id="5e76d-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="5e76d-119">Določite meje programa, ki ga želite konfigurirati za način Internet Explorerja.</span><span class="sxs-lookup"><span data-stu-id="5e76d-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="5e76d-120">Želite vključiti vsa spletna mesta in kontrolnike za splet, ki določajo aplikacijo, ne želite pa vključiti dodatnih mest in kontrolnikov.</span><span class="sxs-lookup"><span data-stu-id="5e76d-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="5e76d-121">Nekatera spletna mesta so morda tako preprosta, kot *https://contoso.com/app1* bi lahko drugi zahtevali, da določite več mest in strani.</span><span class="sxs-lookup"><span data-stu-id="5e76d-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="5e76d-122">Preskusite aplikacijo, da preverite, ali ne deluje izvorno.</span><span class="sxs-lookup"><span data-stu-id="5e76d-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="5e76d-123">Številna spletna mesta ponujajo sodobno vsebino, ko zaznajo sodoben brskalnik in ponudijo le podedovano vsebino, ko zaznajo Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="5e76d-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="5e76d-124">Dodajte program na seznam mesta podjetja, če ne testirate.</span><span class="sxs-lookup"><span data-stu-id="5e76d-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="5e76d-125">Kot najboljšo prakso združite vsa spletna mesta, ki vključujejo program.</span><span class="sxs-lookup"><span data-stu-id="5e76d-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="5e76d-126">Ko nadgradite program, boste lažje odstranili celotno mesto iz načina Internet Explorerja in začeli uporabljati sodoben brskalnik za ta program.</span><span class="sxs-lookup"><span data-stu-id="5e76d-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="5e76d-127">Ko končate z odkrivanjem mesta in analizirate podatke, si lahko ogledate strategijo kanala.</span><span class="sxs-lookup"><span data-stu-id="5e76d-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

