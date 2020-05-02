---
title: Zasebni kanal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005454"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="d16d9-102">Zasebni kanali v storitvi Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d16d9-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="d16d9-103">Zasebni kanali so nova funkcija v storitvi Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="d16d9-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="d16d9-104">Upoštevajte, da zasebnih kanalov ni mogoče pretvoriti iz standardnih kanalov ali obratno.</span><span class="sxs-lookup"><span data-stu-id="d16d9-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="d16d9-105">Za podrobnosti o zasebnih kanalih, kot so informacije o [ustvarjanju zasebnega kanala in članstvu](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) ter na [zasebnih mestih SharePointovih mest](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), si oglejte [zasebne kanale v storitvi Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="d16d9-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="d16d9-106">**Opomba:** Ker konfiguracija za hranjenje zasebnih sporočil kanala še ni podprta, najemniki z omogočenimi pravilniki o hranjenju ne bodo mogli privzeto omogočiti zasebnih kanalov.</span><span class="sxs-lookup"><span data-stu-id="d16d9-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="d16d9-107">Zasebne kanale lahko omogočite v skrbniškem središču ekip.</span><span class="sxs-lookup"><span data-stu-id="d16d9-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="d16d9-108">Upoštevajte tudi, da je hranjenje datotek, ki so v skupni rabi v zasebnih kanalih, medtem ko hranjenje zasebnih sporočil kanala ni podprto.</span><span class="sxs-lookup"><span data-stu-id="d16d9-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="d16d9-109">**Potrebujete novega lastnika ekipe?**</span><span class="sxs-lookup"><span data-stu-id="d16d9-109">**Need a new team owner?**</span></span>

<span data-ttu-id="d16d9-110">Če lastnik zasebnega kanala zapusti, lahko dodate novega lastnika ekipe prek ekipe PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d16d9-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="d16d9-111">Pojdi [tukaj](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) za namestitev ekip PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d16d9-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="d16d9-112">Tukaj je ukaz cmdlet boste potrebovali:</span><span class="sxs-lookup"><span data-stu-id="d16d9-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="d16d9-113">Če želite več informacij o skupini PowerShell, glejte [pregled skupin PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="d16d9-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
