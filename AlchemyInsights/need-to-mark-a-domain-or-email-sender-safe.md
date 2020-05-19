---
title: Potreba označiti domeno ali e-poštni pošiljatelj varno?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281187"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="eb6e7-102">Potreba označiti domeno ali e-poštni pošiljatelj varno?</span><span class="sxs-lookup"><span data-stu-id="eb6e7-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="eb6e7-103">Uporaba **varnih seznamov pošiljateljev ni priporočljiva** , saj odpira vašo organizacijo v spam, Phish, in prevara napadov.</span><span class="sxs-lookup"><span data-stu-id="eb6e7-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="eb6e7-104">Če pa obstaja poslovna zahteva, **priporočamo** , da za to uporabite **[pravila za pretok pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="eb6e7-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="eb6e7-105">Naše smernice zagotavljajo avtentikacijo pošiljatelja (preveri, ali je domena pošiljateljica neponarejena).</span><span class="sxs-lookup"><span data-stu-id="eb6e7-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="eb6e7-106">**Opomba**: ne priporočamo upravljanja lažnih pozitivnih rezultatov z uporabo varnih seznamov pošiljateljev, ker lahko izjeme pri filtriranju neželene pošte odprejo vašo organizacijo z varnostnimi napadi.</span><span class="sxs-lookup"><span data-stu-id="eb6e7-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="eb6e7-107">Če uporabniki prejmejo sporočila, ki so nepravilno označena kot vsiljena ali neželena e-pošta, prosimo, **[prijavite sporočila in datoteke Microsoftu](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="eb6e7-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="eb6e7-108">Varen oddajnik v razgled, omogučiti oddajnik zapisati v seznam, ali omogučiti področje zapisati v seznam v smešen-spam policija **should obstati izogibati se** zato ker oddajnik bypass vsi spam, prevara, ter Phish varstvo, ter oddajnik AUTHENTICATION (SPF, DKIM, dMarc).</span><span class="sxs-lookup"><span data-stu-id="eb6e7-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="eb6e7-109">Ta metoda se najbolje uporablja samo za začasno testiranje.</span><span class="sxs-lookup"><span data-stu-id="eb6e7-109">This method is best used for temporary testing only.</span></span>
