---
title: Pravilniki o hranjenju v Skrbniškem središču za Exchange ne delujejo
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952244"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="86543-102">Pravilniki o hranjenju v Skrbniškem središču za Exchange</span><span class="sxs-lookup"><span data-stu-id="86543-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="86543-103">Če želite, da zaženemo avtomatizirana preverjanja za spodaj omenjene nastavitve, izberite gumb »Nazaj« < – na vrhu te strani in nato vnesite e-poštni naslov uporabnika, ki ima težave s pravilniki o hranjenju.</span><span class="sxs-lookup"><span data-stu-id="86543-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="86543-104">Če imate težave s pravilniki o hranjenju v Skrbniškem središču za Exchange, ki se ne uporabljajo za nabiralnike ali elemente, ki se ne premaknejo v nabiralnik arhiva, preverite to:</span><span class="sxs-lookup"><span data-stu-id="86543-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="86543-105">**Korenski vzroki:**</span><span class="sxs-lookup"><span data-stu-id="86543-105">**Root Causes:**</span></span>

- <span data-ttu-id="86543-106">**Pomočnik za upravljane** mape ni obdelal uporabnikovega nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="86543-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="86543-107">Pomočnik za upravljane mape poskuša obdelati vsak nabiralnik v organizaciji v oblaku enkrat na sedem dni.</span><span class="sxs-lookup"><span data-stu-id="86543-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="86543-108">**Rešitev:** Zaženite pomočnika za upravljane mape.</span><span class="sxs-lookup"><span data-stu-id="86543-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="86543-109">**Zadržanje** hranjenja **je bilo omogočeno** za nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="86543-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="86543-110">Če je bil nabiralnik v zadržanju hranjenja, se v tem času pravilnik o hranjenju za nabiralnik ne bo obdelal.</span><span class="sxs-lookup"><span data-stu-id="86543-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="86543-111">**Rešitev:** Preverite stanje nastavitve zadržanja in po potrebi posodobite.</span><span class="sxs-lookup"><span data-stu-id="86543-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="86543-112">Če želite več informacij, glejte [Zadržanje hranjenja nabiralnika.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="86543-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="86543-113">**Opomba:** Če je nabiralnik manjši od 10 MB, pomočnik za upravljane mape ne bo samodejno obdelal nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="86543-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="86543-114">Če želite več informacij o pravilnikih o hranjenju v Skrbniškem središču za Exchange, glejte:</span><span class="sxs-lookup"><span data-stu-id="86543-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="86543-115">Oznake za hranjenje in pravilniki o hranjenju</span><span class="sxs-lookup"><span data-stu-id="86543-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="86543-116">[Uporaba pravilnika o hranjenju za nabiralnike](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ali [dodajanje ali odstranjevanje oznak za hranjenje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="86543-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="86543-117">Kako prepoznati vrsto zadržanja v nabiralniku</span><span class="sxs-lookup"><span data-stu-id="86543-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
