---
title: 2491 opozorilo email sporočila od soseda podal zaradi najemnika ali uporabnika preglasijo politike
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391532"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="49d69-102">Opozorilo email sporočila od soseda podal zaradi najemnika ali uporabnika preglasijo politike</span><span class="sxs-lookup"><span data-stu-id="49d69-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="49d69-103">Privzeti opozorilo pravilnik, imenovan "Soseda ki zaradi najemnika ali uporabnika preglasijo" has been valjan jasno najemnikom z Office 365 ATP P1 in P2 licence.</span><span class="sxs-lookup"><span data-stu-id="49d69-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="49d69-104">Če ste prejeli to opozorilo, tukaj so koraki za preiskavo:</span><span class="sxs-lookup"><span data-stu-id="49d69-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="49d69-105">Opozorilo, kliknite **Pogled opozorilo** **opozoril** stran v varnostno & Center skladnosti.</span><span class="sxs-lookup"><span data-stu-id="49d69-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="49d69-106">Izberite Zvoni za prikaz možnost **pogleda seznama sporočil** ali **sporočil pogled v Explorerju**.</span><span class="sxs-lookup"><span data-stu-id="49d69-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="49d69-107">Obe možnosti popeljal do podrobnosti sporočila, ki vključuje sporočilo ID.</span><span class="sxs-lookup"><span data-stu-id="49d69-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="49d69-108">Upoštevajte, da bo Threat Explorerju povezavo samodejno filtriranje sporočil, ki ustrezajo alarmna kriterije.</span><span class="sxs-lookup"><span data-stu-id="49d69-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="49d69-109">Morda boste morali prilagoditi filter datuma v Threat Explorerju.</span><span class="sxs-lookup"><span data-stu-id="49d69-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="49d69-110">Lažno sporočilo je bilo dostavljeno zaradi ročno konfigurirane prednost:</span><span class="sxs-lookup"><span data-stu-id="49d69-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="49d69-111">Dovoljeno pošiljatelja ali domene, ki ga uporabnik.</span><span class="sxs-lookup"><span data-stu-id="49d69-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="49d69-112">Dovoljeno pošiljatelja ali domene, ki jih admin polica, smešen-spam.</span><span class="sxs-lookup"><span data-stu-id="49d69-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="49d69-113">Dovoljeno IP naslov v povezavo filter politike.</span><span class="sxs-lookup"><span data-stu-id="49d69-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="49d69-114">A tok pravilo za pošto (znan tudi kot pravila prenosa) ki je konfiguriran, da sporočila v.</span><span class="sxs-lookup"><span data-stu-id="49d69-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="49d69-115">Če menite, da je sporočilo je bilo napačno označeno kot phish, uporabite Outlook [sporočilo poročila povečati-v](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) predloži vzorce sporočilo v mikroskop.</span><span class="sxs-lookup"><span data-stu-id="49d69-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
