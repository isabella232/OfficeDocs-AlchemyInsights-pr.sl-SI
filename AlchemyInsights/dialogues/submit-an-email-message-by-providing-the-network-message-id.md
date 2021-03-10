---
title: Pošiljanje e-poštnega sporočila z zagotavljanjem ID-ja omrežnega sporočila
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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695381"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="a3004-102">Pošiljanje e-poštnega sporočila z zagotavljanjem ID-ja omrežnega sporočila</span><span class="sxs-lookup"><span data-stu-id="a3004-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="a3004-103">V **novi oddaji** flyout izberite **e-pošta** in **omrežni ID sporočila**.</span><span class="sxs-lookup"><span data-stu-id="a3004-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="a3004-104">Če želite poiskati ID sporočila za e-poštno sporočilo v Outlooku, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="a3004-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="a3004-105">Dvokliknite e-poštno sporočilo, da ga odprete.</span><span class="sxs-lookup"><span data-stu-id="a3004-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="a3004-106">Izberite   >  **lastnosti** datoteke.</span><span class="sxs-lookup"><span data-stu-id="a3004-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="a3004-107">Odprite beležnico ali prazen Wordov dokument in nato kopirajte in prilepite vsebino, ki je na voljo v polju **Internetne glave** , v odprt dokument za boljšo vidljivost.</span><span class="sxs-lookup"><span data-stu-id="a3004-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="a3004-108">Poiščite polje **X-MS-Exchange-Organization-Network-ID sporočila** .</span><span class="sxs-lookup"><span data-stu-id="a3004-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="a3004-109">Vrednost za **:** je ID, ki ga potrebujete za vašo predložitvi.</span><span class="sxs-lookup"><span data-stu-id="a3004-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="a3004-110">V razdelku **prejemniki**, če je e-pošta, iztovorjena v mapi» Neželena pošta «za vse prejemnike te e-pošte, izberite **Izberi vse**.</span><span class="sxs-lookup"><span data-stu-id="a3004-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="a3004-111">Če niste, izberite le uporabnik, ki je sporočil težavo.</span><span class="sxs-lookup"><span data-stu-id="a3004-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="a3004-112">V **razdelku razlog za pošiljanje**, če ste izbrali **bi morali biti blokirani**, določite, ali naj bo sporočilo blokirano kot **neželena pošta**, **lažno predstavljanje** ali **zlonamerna programska oprema**, nato pa izberite **Pošlji**.</span><span class="sxs-lookup"><span data-stu-id="a3004-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="a3004-113">Če želite izvedeti več, glejte [pošiljanje domnevnih neželene pošte, Phish, URL-jev in datotek Microsoftu za skeniranje](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="a3004-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
