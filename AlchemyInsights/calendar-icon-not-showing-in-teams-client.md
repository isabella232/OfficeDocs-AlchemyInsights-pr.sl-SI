---
title: Ikona koledarja ni prikazana v odjemalcu aplikacije Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819969"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="2bee2-102">Ikona koledarja ni prikazana v odjemalcu aplikacije Teams</span><span class="sxs-lookup"><span data-stu-id="2bee2-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="2bee2-103">Zavihek »Koledar« v aplikaciji Teams zahteva dostop do nabiralnika Exchange prek storitev Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="2bee2-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="2bee2-104">Nabiralnik Exchange je lahko v spletu ali na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="2bee2-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="2bee2-105">Za spletne uporabnike, ki ne vidijo zavihka »Koledar«, preverite, [ali imajo licenco za nabiralnik Exchange Online in ali je nabiralnik omogočen](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="2bee2-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="2bee2-106">Če ima uporabnik veljaven nabiralnik v storitvi Exchange Online, vendar še vedno ne vidi zavihka »Koledar«, je morda prišlo do težave z omrežjem.</span><span class="sxs-lookup"><span data-stu-id="2bee2-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="2bee2-107">Uporabite [Microsoftov analizator oddaljene povezljivosti](https://testconnectivity.microsoft.com/) in zaženite **preskuse povezljivosti z Microsoft Exchangeevimi spletnimi storitvami** za prizadetega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="2bee2-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="2bee2-108">Na koncu preverite še [Aplikacije Teams – pravilniki o nastavitvah aplikacij](https://admin.teams.microsoft.com/policies/app-setup) in se prepričajte, da aplikacija Koledar ni bila odstranjena iz pravilnika, uporabljenega za uporabnika (najverjetneje **Globalno (privzeto na ravni celotne organizacije)**.</span><span class="sxs-lookup"><span data-stu-id="2bee2-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="2bee2-109">Če vaši uporabniki uporabljajo aplikacije na mestu uporabe, morate preveriti, ali je hibridna konfiguracija ustrezna.</span><span class="sxs-lookup"><span data-stu-id="2bee2-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="2bee2-110">Za odpravljanje težav uporabite [čarovnika za hibridno konfiguracijo](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="2bee2-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="2bee2-111">Imejte v mislih, da [aplikacija Teams zahteva Exchange 2016 CU3 ali višje](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="2bee2-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
