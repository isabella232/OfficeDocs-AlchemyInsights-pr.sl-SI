---
title: Prepoznavanje dogodkov brisanja sporočil v dnevnikih revizij
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716512"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="42e24-102">Dnevniki revizij za izbrisana e-poštna sporočila</span><span class="sxs-lookup"><span data-stu-id="42e24-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="42e24-103">Od januarja 2019 se Microsoft samodejno obrača na beleženje dnevnika nadzora nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="42e24-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="42e24-104">V nasprotnem primeru, če želite pregledati brisanje dogodkov sporočila za določenega uporabnika, morate ročno omogočiti brisanje dejanj za nadzor.</span><span class="sxs-lookup"><span data-stu-id="42e24-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="42e24-105">Če je beleženje revizij nabiralnika že omogočeno za vašo organizacijo ali za določenega uporabnika, sledite spodnjim korakom.</span><span class="sxs-lookup"><span data-stu-id="42e24-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="42e24-106">Prijavite se v [Microsoft 365 Security & center za skladnost](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="42e24-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="42e24-107">Kliknite **iskanje in preiskovanje** ter izberite **iskanje dnevnika revizij**.</span><span class="sxs-lookup"><span data-stu-id="42e24-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="42e24-108">Izberite časovno območje v polji **Začetni datum** in **končni datum** .</span><span class="sxs-lookup"><span data-stu-id="42e24-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="42e24-109">Določite uporabniško ime za uporabnika, ki ga želite raziskati (uporabnik, ki je izbrisal elemente).</span><span class="sxs-lookup"><span data-stu-id="42e24-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="42e24-110">V polju **dejavnosti** izberite **izbrisana sporočila iz mape» izbrisani predmeti «** in **premaknjena sporočila v mapo» izbrisani predmeti «**.</span><span class="sxs-lookup"><span data-stu-id="42e24-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="42e24-111">Kliknite **Iskanje**.</span><span class="sxs-lookup"><span data-stu-id="42e24-111">Click **Search**.</span></span>

<span data-ttu-id="42e24-112">V rezultatih Izberite zapis o reviziji.</span><span class="sxs-lookup"><span data-stu-id="42e24-112">In the results, select an audit record.</span></span> <span data-ttu-id="42e24-113">V meniju podrobnosti kliknite **več informacij**.</span><span class="sxs-lookup"><span data-stu-id="42e24-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="42e24-114">Dodatne informacije o izbrisanem elementu (na primer vrstica z zadevo in mesto elementa, ko je bil izbrisan) so prikazane v polju» **Affecteditems** «.</span><span class="sxs-lookup"><span data-stu-id="42e24-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="42e24-115">Lastnost **Clientinfostring** bo pokazala, ali je prišlo do brisanja v Outlooku, Outlooku v spletu (prej znan kot Outlook Web App) ali kateri koli drugi napravi.</span><span class="sxs-lookup"><span data-stu-id="42e24-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="42e24-116">Če želite več informacij, glejte [določanje, kdo je nastavil posredovanje e-pošte za nabiralnik](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="42e24-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="42e24-117">**Opomba**: izbrisanih elementov ni mogoče pridobiti z uporabo funkcije dnevnika revizij.</span><span class="sxs-lookup"><span data-stu-id="42e24-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="42e24-118">Če želite pridobiti izbrisana sporočila v Outlooku v spletu, glejte [obnovitev izbrisanih elementov v storitvi Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="42e24-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
