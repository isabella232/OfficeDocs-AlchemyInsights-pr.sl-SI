---
title: Dostop do naročnine
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807722"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="53e31-102">Ne morem se vpisati v Azure zaradi težav z brskalnikom (brskalnik se obesi, se vrti, ne naloži, itd.)</span><span class="sxs-lookup"><span data-stu-id="53e31-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="53e31-103">Morda boste vplivali na izpad.</span><span class="sxs-lookup"><span data-stu-id="53e31-103">You might be impacted by an outage.</span></span> <span data-ttu-id="53e31-104">Preverite, ali je prišlo do trajnega izpada: [stanje Azure Health](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="53e31-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="53e31-105">Odjavite se iz vseh aktivnih sej v storitvi Azure.</span><span class="sxs-lookup"><span data-stu-id="53e31-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="53e31-106">Začnite v zasebnem ali načinu brez beleženja zgodovine v spletnem brskalniku.</span><span class="sxs-lookup"><span data-stu-id="53e31-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="53e31-107">Lahko tudi poskusite osvežiti brskalnik, uporabite drug brskalnik, izbrišete piškotke predpomnilnika, če zgoraj ne deluje.</span><span class="sxs-lookup"><span data-stu-id="53e31-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="53e31-108">Več informacij: [Odpravljanje težav z vpisom](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="53e31-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="53e31-109">**Dostop do naročnin ni mogoč**</span><span class="sxs-lookup"><span data-stu-id="53e31-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="53e31-110">V [portalu Azure](https://portal.azure.com/)se prepričajte, da je na računu v zgornjem desnem kotu izbran pravilen imenik Azure.</span><span class="sxs-lookup"><span data-stu-id="53e31-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="53e31-111">V [središču za Azure Account (račun](https://account.windowsazure.com/Subscriptions)) se prepričajte, ali je račun uporabljen pri skrbniku računa.</span><span class="sxs-lookup"><span data-stu-id="53e31-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="53e31-112">Več informacij: [Odpravljanje težav z naročnino](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="53e31-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="53e31-113">**Dostop do zgodovine obračunavanja ni mogoč**</span><span class="sxs-lookup"><span data-stu-id="53e31-113">**Unable to access billing history**</span></span>

<span data-ttu-id="53e31-114">Skrbnik računa mora preveriti, ali je uporabnik, ki dostopa do informacij o obračunavanju, dodan v imeniku Azure Active Directory kot gostujoči uporabnik: [Dodajanje ali brisanje novega uporabnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="53e31-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="53e31-115">Uporabnik mora nato dati globalno skrbniško vlogo: [dodeliti vlogo uporabnikom](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="53e31-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="53e31-116">Objavite to, uporabniku je mogoče dodeliti dostop do obračunavanja s pravilniki RBAC: [dodeljevanje dostopa do obračunavanja](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="53e31-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="53e31-117">**Priporočeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="53e31-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="53e31-118">Ne morem se vpisati v upravljanje moje naročnine na Azure</span><span class="sxs-lookup"><span data-stu-id="53e31-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)