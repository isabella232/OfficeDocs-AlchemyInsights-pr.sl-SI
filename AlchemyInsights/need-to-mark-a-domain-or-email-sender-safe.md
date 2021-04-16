---
title: Ali morate označiti domeno ali pošiljatelja e-pošte varno?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792148"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="f5119-102">Ali morate označiti domeno ali pošiljatelja e-pošte varno?</span><span class="sxs-lookup"><span data-stu-id="f5119-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="f5119-103">Uporaba seznamov **varnih pošiljateljev ni** priporočljiva, saj v vaši organizaciji odpre napad za neželeno pošto, lažno predstavljanje in lažno predstavljanje.</span><span class="sxs-lookup"><span data-stu-id="f5119-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="f5119-104">Če pa obstajajo poslovne zahteve, priporočamo, **da za** to uporabite **[pravila](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** toka pošte.</span><span class="sxs-lookup"><span data-stu-id="f5119-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="f5119-105">Z našimi navodili je mogoče zagotoviti, da je preverjanje pristnosti pošiljatelja (preverjanje, da ni ponarejena domena).</span><span class="sxs-lookup"><span data-stu-id="f5119-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="f5119-106">**Opomba:** Priporočamo, da ne upravljate napačne pozitivne pošte z uporabo seznamov varnih pošiljateljev, saj lahko izjeme pri filtriranju neželene pošte odprejo organizacijo do varnostnih napadov.</span><span class="sxs-lookup"><span data-stu-id="f5119-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="f5119-107">Če vaši uporabniki prejmejo sporočila, ki so nepravilno označena kot neželena ali neželena e-pošta, prijavite **[sporočila in datoteke Microsoftu.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="f5119-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="f5119-108">Varnim pošiljateljem v Outlooku, seznamu dovoljenih pošiljateljev  ali seznamu dovoljenih domen v pravilnikih za preprečevanje neželene pošte se je treba izogniti, saj pošiljatelji zaobidejo vso neželeno pošto, zaščito pred lažjo zaščito in preverjanje pristnosti pošiljatelja (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="f5119-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="f5119-109">Ta način je najboljši za začasno preskušanje.</span><span class="sxs-lookup"><span data-stu-id="f5119-109">This method is best used for temporary testing only.</span></span>
