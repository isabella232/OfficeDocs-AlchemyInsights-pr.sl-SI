---
title: Zaščita pred napadom na ponarejenimi pošiljatelji
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037179"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="e0218-102">Zaščita pred napadom na ponarejenimi pošiljatelji</span><span class="sxs-lookup"><span data-stu-id="e0218-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="e0218-103">Ponarejenimi pošiljatelji je poročila o neuspeli dostavi (znana tudi kot NDR ali Bounce messages), ki jih prejmete za sporočila, ki jih niste poslali.</span><span class="sxs-lookup"><span data-stu-id="e0218-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="e0218-104">Pošiljatelji neželene pošte ponarejali (spoof) **od:** naslov svojih sporočil in pogosto uporabljajo realne e-poštne naslove, ki posojajo verodostojnost njihovim sporočilom.</span><span class="sxs-lookup"><span data-stu-id="e0218-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="e0218-105">Če pošiljatelji neželene pošte neizogibno pošiljajo sporočila neobstoječim prejemnikom, je ciljni e-poštni strežnik v glavnem Prelisičil, da vrne sporočilo, ki ga ni mogoče dostaviti, v poročilo o dostopu do ponarejenega pošiljatelja v naslovu **od:** .</span><span class="sxs-lookup"><span data-stu-id="e0218-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="e0218-106">Dodatne informacije najdete v [ponarejenimi pošiljatelji v](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)storitvi EOP.</span><span class="sxs-lookup"><span data-stu-id="e0218-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="e0218-107">**Omogočanje zaščite ponarejenimi pošiljatelji**</span><span class="sxs-lookup"><span data-stu-id="e0218-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="e0218-108">Če želite omogočiti zaščito pred ponarejenimi pošiljatelji, sledi spodnji poti.</span><span class="sxs-lookup"><span data-stu-id="e0218-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="e0218-109">**protection.office.com > obvladovanja groženj > pravilnik > antispam > izberite pravilnik filtra neželene pošte in urejanje pravilnika > lastnosti neželene pošte > označi kot neželeno pošto > NDR ponarejenimi pošiljatelji > jo nastavite na» on «.**</span><span class="sxs-lookup"><span data-stu-id="e0218-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="e0218-110">Če menite, da je bil račun ogrožen, si oglejte to:</span><span class="sxs-lookup"><span data-stu-id="e0218-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="e0218-111">Odziv na ogrožene e-poštne račune</span><span class="sxs-lookup"><span data-stu-id="e0218-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="e0218-112">Odstranjevanje blokiranih uporabnikov iz portala omejenih uporabnikov v storitvi Office 365</span><span class="sxs-lookup"><span data-stu-id="e0218-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



