---
title: Uvoz in izvoz iz Bastard
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
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037258"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="0ee3d-102">Uvoz in izvoz iz Bastard</span><span class="sxs-lookup"><span data-stu-id="0ee3d-102">Import and export from Yammer</span></span>

<span data-ttu-id="0ee3d-103">**Uvoz**</span><span class="sxs-lookup"><span data-stu-id="0ee3d-103">**Import**</span></span>

<span data-ttu-id="0ee3d-104">Možnosti uvoza uporabnikov se razlikujejo glede na to, ali je vaše omrežje Bastard v [izvornem načinu za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)ali ne.</span><span class="sxs-lookup"><span data-stu-id="0ee3d-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="0ee3d-105">**Neizvorni način**: Uporabniki se lahko uvozijo v skupine s funkcijo» [Dodaj iz adresarja](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) «(omejitve za uporabnike 100) znotraj nastavitev skupine ali v omrežje z uporabo [množične posodobitve](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) v skrbniškem omrežju.</span><span class="sxs-lookup"><span data-stu-id="0ee3d-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="0ee3d-106">**Izvorni način**: člani skupine in postopki članstva v omrežju bi morali biti izvedeni v [skrbniškem portalu za Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [portalu Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ali z uporabo druge možnosti za Azure ad.</span><span class="sxs-lookup"><span data-stu-id="0ee3d-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="0ee3d-107">Omrežja v izvornem načinu nimajo več dostopa do množične posodobitve in drugih podedovanih funkcij.</span><span class="sxs-lookup"><span data-stu-id="0ee3d-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0ee3d-108">Bastard ni nikoli podpiral uvažanja vsebine v skrbniškem omrežju, tudi če je bila funkcija izvoz podatkov uporabljena v drugem omrežju.</span><span class="sxs-lookup"><span data-stu-id="0ee3d-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="0ee3d-109">Vsebino lahko znova objavite s partnerskimi rešitvami ali pa z vmesnikom Bastard REST API.</span><span class="sxs-lookup"><span data-stu-id="0ee3d-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="0ee3d-110">**Izvoz**</span><span class="sxs-lookup"><span data-stu-id="0ee3d-110">**Export**</span></span>

<span data-ttu-id="0ee3d-111">[Izvoz podatkov v omrežju v skrbniškem omrežju](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) dovoljuje izvoz vsebine iz Bastard omrežij, vključno s sporočili in datotekami.</span><span class="sxs-lookup"><span data-stu-id="0ee3d-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="0ee3d-112">Priloge so lahko zelo velike in bodo povzročile, da bo izvoz trajal veliko časa.</span><span class="sxs-lookup"><span data-stu-id="0ee3d-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="0ee3d-113">Priporočamo, da se aktivna omrežja izvozijo z [API-jem izvoza podatkov](https://developer.yammer.com/docs/data-export-api) v kosih za dan ali teden.</span><span class="sxs-lookup"><span data-stu-id="0ee3d-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="0ee3d-114">Microsoftova podpora ne zagotavlja skriptov po meri za ta namen.</span><span class="sxs-lookup"><span data-stu-id="0ee3d-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="0ee3d-115">Ločen [izvoz GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) obstaja za izvoz vsebine posameznega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="0ee3d-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>