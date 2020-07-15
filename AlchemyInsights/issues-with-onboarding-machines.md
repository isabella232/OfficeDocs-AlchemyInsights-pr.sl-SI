---
title: Težave z uvajanje stroji
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141661"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="2bde3-102">Težave z uvajanje stroji</span><span class="sxs-lookup"><span data-stu-id="2bde3-102">Issues with onboarding machines</span></span>

<span data-ttu-id="2bde3-103">Morda imate težave z napravami za vkrcavanje na storitev MDATP.</span><span class="sxs-lookup"><span data-stu-id="2bde3-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="2bde3-104">Če lahko dostopate do stroja za končnega uporabnika, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="2bde3-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="2bde3-105">Prenesite diagnostično orodje [analizatorja povezljivosti odjemalca](https://aka.ms/mdatpanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="2bde3-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="2bde3-106">Citat ter prost dostop MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="2bde3-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="2bde3-107">Poiščite diagnostični dnevnik v mapi z imenom MDATPClientAnalyzerResult, isto mapo, kjer je orodje za analizo preneseno.</span><span class="sxs-lookup"><span data-stu-id="2bde3-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="2bde3-108">Preglejte dnevniško datoteko, MDATPClientAnalyzer.txt, da poiščete težave z nastavitvami povezljivosti ali internetne proxy.</span><span class="sxs-lookup"><span data-stu-id="2bde3-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>