---
title: Prepoznavanje posredovanje zunanji e-poštni nabiralniki v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539117"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="56bb9-102">Ko zunanje email odpošiljanje konfiguriran na nabiralnike</span><span class="sxs-lookup"><span data-stu-id="56bb9-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="56bb9-103">Ko Office 365 uporabnik konfigurira posredovanje zunanji e-poštni nabiralnik, se nadzoruje dejavnosti kot del ukaza »cmdlet« **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="56bb9-103">When an Office 365  user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="56bb9-104">Si lahko ogledate uporabo revizijskih dnevnik iskanja v varnostno & Center skladnosti dejavnosti.</span><span class="sxs-lookup"><span data-stu-id="56bb9-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="56bb9-105">Prijavite se v [Office 365 varnost & skladnosti Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="56bb9-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="56bb9-106">Pojdi na **Iskanje** > **revizije dnevnik iskalna** stran.</span><span class="sxs-lookup"><span data-stu-id="56bb9-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="56bb9-107">Izberite datumski obseg v polji **Začetni datum** in **končni datum** .</span><span class="sxs-lookup"><span data-stu-id="56bb9-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="56bb9-108">Vam ni treba navesti uporabniško ime.</span><span class="sxs-lookup"><span data-stu-id="56bb9-108">You don't need to specify a username.</span></span> <span data-ttu-id="56bb9-109">Preverite, ali je polje **dejavnosti** nastavite pokazati **rezultate za vse dejavnosti**.</span><span class="sxs-lookup"><span data-stu-id="56bb9-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="56bb9-110">Kliknite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="56bb9-110">Click **Search**.</span></span>

<span data-ttu-id="56bb9-111">Na seznamu rezultatov kliknite **Filter rezultatov** in vnesite **Set-Mailbox** v precejalo škatla dejavnost.</span><span class="sxs-lookup"><span data-stu-id="56bb9-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="56bb9-112">Izberite revizijski zapis v rezultatih.</span><span class="sxs-lookup"><span data-stu-id="56bb9-112">Select an audit record in the results.</span></span> <span data-ttu-id="56bb9-113">V pojavni meni **podrobnosti** , kliknite **več informacij**.</span><span class="sxs-lookup"><span data-stu-id="56bb9-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="56bb9-114">Moraš pogledati podrobnosti o vsaki revizijski zapis ugotoviti, če je dejavnost povezana z email odpošiljanje.</span><span class="sxs-lookup"><span data-stu-id="56bb9-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="56bb9-115">**ObjectId**: vrednost Vzdevek nabiralnika, ki je bila spremenjena.</span><span class="sxs-lookup"><span data-stu-id="56bb9-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="56bb9-116">**Parametri**: _ForwardingSmtpAddress_ označuje ciljni e-poštni naslov.</span><span class="sxs-lookup"><span data-stu-id="56bb9-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="56bb9-117">**ID uporabnika**: uporabnika, ki je konfiguriran posredovanje e-pošte v nabiralniku **ObjectId** področju.</span><span class="sxs-lookup"><span data-stu-id="56bb9-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="56bb9-118">Če želite več informacij, glejte [določanje ki nastaviti e-pošte, posredovanje za nabiralnik](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="56bb9-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
