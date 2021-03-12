---
title: Oddaljeno odpravljanje težav z napravami s sistemom Windows 10 za napredna zaščita pred grožnjami
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750043"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="71e27-102">Oddaljeno odpravljanje težav z napravami s sistemom Windows 10 za napredna zaščita pred grožnjami</span><span class="sxs-lookup"><span data-stu-id="71e27-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="71e27-103">Če lahko dostopate do oddaljenega računalnika, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="71e27-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="71e27-104">Prenesite diagnostično orodje [analizator povezljivosti odjemalca](https://go.microsoft.com/fwlink/?linkid=2143466) .</span><span class="sxs-lookup"><span data-stu-id="71e27-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="71e27-105">Ekstrahirajte in zaženite MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="71e27-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="71e27-106">Poiščite diagnostični dnevnik v mapi MDATPClientAnalyzerResult, ki je ista mapa, v kateri je bilo preneseno orodje analizatorja.</span><span class="sxs-lookup"><span data-stu-id="71e27-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="71e27-107">Če želite poiskati težave s povezljivostjo ali nastavitvami internetnega proxyja, Preglejte dnevniško datoteko MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="71e27-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="71e27-108">Če želite izvedeti več, glejte [težave s stroji za vkrcanje](https://go.microsoft.com/fwlink/?linkid=2143634).</span><span class="sxs-lookup"><span data-stu-id="71e27-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
