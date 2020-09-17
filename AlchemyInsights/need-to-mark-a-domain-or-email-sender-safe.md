---
title: Ali želite označiti varno domeno ali pošiljatelja e-pošte?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803261"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="df829-102">Ali želite označiti varno domeno ali pošiljatelja e-pošte?</span><span class="sxs-lookup"><span data-stu-id="df829-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="df829-103">Uporaba **seznamov varnih pošiljateljev ni priporočljiva** , saj vaša organizacija odpre vašo organizacijo za neželeno pošto, Phish in lažne napade.</span><span class="sxs-lookup"><span data-stu-id="df829-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="df829-104">Če pa obstaja poslovna zahteva, **priporočamo** , da za to uporabite **[pravila za tok pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="df829-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="df829-105">Naše vodilo zagotavlja preverjanje pristnosti pošiljatelja (preveri, ali je domena za pošiljanje lažna).</span><span class="sxs-lookup"><span data-stu-id="df829-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="df829-106">**Opomba**: ne priporočamo, da na seznamih varnih pošiljateljev uporabite lažne pozitivne izraze, ker lahko izjeme do filtriranja neželene pošte odprejo vašo organizacijo na varnostne napade.</span><span class="sxs-lookup"><span data-stu-id="df829-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="df829-107">Če vaši uporabniki prejmejo sporočila nepravilno označena kot neželena ali neželena e-pošta, pošljite **[Microsoftu sporočila o sporočilih in datotekah](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="df829-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="df829-108">Varni pošiljatelji v Outlooku, dovoljen seznam pošiljatelja ali dovoljen seznam domen v pravilnikih za preprečevanje neželene pošte se **morajo izogibati** , ker pošiljatelji zaobidejo vse neželene pošte, spoof in Phish zaščito ter preverjanje pristnosti pošiljatelja (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="df829-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="df829-109">Ta način je najbolje uporabiti le za začasno testiranje.</span><span class="sxs-lookup"><span data-stu-id="df829-109">This method is best used for temporary testing only.</span></span>
