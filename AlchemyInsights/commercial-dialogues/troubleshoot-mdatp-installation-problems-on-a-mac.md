---
title: Odpravljanje težav z namestitvijo MDATP v računalniku Mac
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749768"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="000dc-102">Odpravljanje težav z namestitvijo MDATP v računalniku Mac</span><span class="sxs-lookup"><span data-stu-id="000dc-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="000dc-103">Če Ročna namestitev ni uspešna, se na strani s **povzetkom** čarovnika za namestitev prikaže to sporočilo o napaki:</span><span class="sxs-lookup"><span data-stu-id="000dc-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="000dc-104">» Prišlo je do napake med namestitvijo.</span><span class="sxs-lookup"><span data-stu-id="000dc-104">"An error occurred during installation.</span></span> <span data-ttu-id="000dc-105">Namestitveni program je zaznal napako, zaradi katere namestitev ni uspela.</span><span class="sxs-lookup"><span data-stu-id="000dc-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="000dc-106">Za pomoč se obrnite na izdelovalca programske opreme. "</span><span class="sxs-lookup"><span data-stu-id="000dc-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="000dc-107">Za uvajanje MDM na strani je prikazana tudi splošna napaka namestitve.</span><span class="sxs-lookup"><span data-stu-id="000dc-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="000dc-108">Čeprav ne prikazujemo natančnih napak za končne uporabnike, bomo obdržali dnevniško datoteko z napredkom namestitve v **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="000dc-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="000dc-109">Vsako sejo namestitve priloži tej dnevniški datoteki.</span><span class="sxs-lookup"><span data-stu-id="000dc-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="000dc-110">Če želite izključiti le zadnjo sejo namestitve, uporabite `sed` .</span><span class="sxs-lookup"><span data-stu-id="000dc-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="000dc-111">Če želite izvedeti več, glejte [Odpravljanje težav z namestitvijo za Microsoft DEFENDER ATP za Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="000dc-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
