---
title: Prepoznavanje Izbriši sporočilo dogodkov v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909561"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="50ff2-102">Dnevnikov za izbrisati email vest</span><span class="sxs-lookup"><span data-stu-id="50ff2-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="50ff2-103">Odhod v januarju 2019, Microsoft zavija na nabiralnik revizije prijavi privzeto.</span><span class="sxs-lookup"><span data-stu-id="50ff2-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="50ff2-104">Drugače, pregled izbrisati sporočilo dogodkov za določenega uporabnika, boste morali ročno omogočiti dejanja delete za revidiranje.</span><span class="sxs-lookup"><span data-stu-id="50ff2-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="50ff2-105">Če nabiralnik revizijo pisanje dnevnika je že omogočeno za organizacijo ali za določenega uporabnika, sledite spodnjim korakom.</span><span class="sxs-lookup"><span data-stu-id="50ff2-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="50ff2-106">Prijavite se v [Office 365 varnost & skladnosti Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="50ff2-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="50ff2-107">Kliknite **Išči ter preiskave** in izberite **Išči dnevnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="50ff2-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="50ff2-108">Izberite datumski obseg v polji **Začetni datum** in **končni datum** .</span><span class="sxs-lookup"><span data-stu-id="50ff2-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="50ff2-109">Določite uporabniško ime uporabnika, ki jo želite raziskati (uporabnik, ki je izbrisano).</span><span class="sxs-lookup"><span data-stu-id="50ff2-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="50ff2-110">Na področju **dejavnosti** , izberite **izbrisana sporočila iz mape Izbrisano** in **premaknjeno sporočila v mapo Izbrisano**.</span><span class="sxs-lookup"><span data-stu-id="50ff2-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="50ff2-111">Kliknite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="50ff2-111">Click **Search**.</span></span>

<span data-ttu-id="50ff2-112">V rezultate, izberite revizijski zapis.</span><span class="sxs-lookup"><span data-stu-id="50ff2-112">In the results, select an audit record.</span></span> <span data-ttu-id="50ff2-113">V pojavni meni podrobnosti, kliknite **Več informacij**.</span><span class="sxs-lookup"><span data-stu-id="50ff2-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="50ff2-114">Dodatne informacije o izbrisanega elementa (na primer, zadevo in mesto elementa, ko je bila izbrisana) je prikazana v polju **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="50ff2-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="50ff2-115">Lastnost **ClientInfoString** prikaže, če izbris je prišlo v Outlooku, Outlook v spletu (prej znan kot Outlook Web App), ali katere koli druge naprave.</span><span class="sxs-lookup"><span data-stu-id="50ff2-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="50ff2-116">Če želite več informacij, glejte [določanje ki nastaviti e-pošte, posredovanje za nabiralnik](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="50ff2-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="50ff2-117">**Opomba**: ne more pridobiti izbrisano funkcijo dnevnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="50ff2-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="50ff2-118">Če naložite izbrisana sporočila v Outlook v spletu, glejte [obnavljanje izbrisanih elementov v storitvi Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="50ff2-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
