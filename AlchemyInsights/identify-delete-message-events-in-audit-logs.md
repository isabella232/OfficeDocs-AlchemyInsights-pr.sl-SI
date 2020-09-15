---
title: Prepoznavanje dogodkov brisanja sporočil v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696529"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="e9fd5-102">Dnevniki nadzora za izbrisana e-poštna sporočila</span><span class="sxs-lookup"><span data-stu-id="e9fd5-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="e9fd5-103">Z začetkom januarja 2019 se Microsoft samodejno vklopi v dnevnik nadzora nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="e9fd5-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="e9fd5-104">V nasprotnem primeru za pregled brisanja dogodkov sporočila za določenega uporabnika morate ročno omogočiti dejanja brisanja za nadzor.</span><span class="sxs-lookup"><span data-stu-id="e9fd5-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="e9fd5-105">Če je pisanje dnevnika nadzora nabiralnika že omogočeno za vašo organizacijo ali za določenega uporabnika, upoštevajte spodnja navodila.</span><span class="sxs-lookup"><span data-stu-id="e9fd5-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="e9fd5-106">Prijavite se v [središče za varnost & skladnost s predpisi Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="e9fd5-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="e9fd5-107">Kliknite **iskanje in preiskovanje** in izberite **iskanje dnevnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="e9fd5-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="e9fd5-108">Izberite datumski obseg v poljih **Začetni datum** in **končni datum** .</span><span class="sxs-lookup"><span data-stu-id="e9fd5-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="e9fd5-109">Določite uporabniško ime za uporabnika, ki ga želite raziskati (uporabnik, ki je izbrisal elemente).</span><span class="sxs-lookup"><span data-stu-id="e9fd5-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="e9fd5-110">V polju **dejavnosti** izberite **izbrisana sporočila iz mape» Izbrisano «** in **premaknjena sporočila v mapo» Izbrisano «**.</span><span class="sxs-lookup"><span data-stu-id="e9fd5-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="e9fd5-111">Kliknite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="e9fd5-111">Click **Search**.</span></span>

<span data-ttu-id="e9fd5-112">V rezultatih Izberite zapis nadzora.</span><span class="sxs-lookup"><span data-stu-id="e9fd5-112">In the results, select an audit record.</span></span> <span data-ttu-id="e9fd5-113">V razdelku podrobnosti flyout kliknite **več informacij**.</span><span class="sxs-lookup"><span data-stu-id="e9fd5-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="e9fd5-114">Dodatne informacije o izbrisanem elementu (na primer vrstica z zadevo in lokacija elementa, ko je bila izbrisana) je prikazana v polju» **AffectedItems** «.</span><span class="sxs-lookup"><span data-stu-id="e9fd5-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="e9fd5-115">Lastnost **ClientInfoString** se prikaže, če je prišlo do brisanja v Outlooku, Outlooku v spletu (prej znan kot Outlook Web App) ali kateri koli drugi napravi.</span><span class="sxs-lookup"><span data-stu-id="e9fd5-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="e9fd5-116">Če želite več informacij, glejte [določanje, kdo je nastavil posredovanje e-pošte za nabiralnik](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="e9fd5-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="e9fd5-117">**Opomba**: izbrisanih elementov ne morete pridobiti s funkcijo dnevnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="e9fd5-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="e9fd5-118">Če želite pridobiti izbrisana sporočila v Outlooku v spletu, [si oglejte obnovitev izbrisanih elementov v programu Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="e9fd5-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
