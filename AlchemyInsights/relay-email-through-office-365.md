---
title: Posredovanje e-pošte prek okolja Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809671"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="347e1-102">Nastavite večfunkcijsko napravo ali aplikacijo za pošiljanje e-pošte</span><span class="sxs-lookup"><span data-stu-id="347e1-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="347e1-103">Več informacij o možnostih in navodila najdete v članku [Nastavitev večfunkcijske naprave ali aplikacije za pošiljanje e-pošte z okoljem Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="347e1-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="347e1-104">**Opomba:** če imate napravo ali aplikacijo, ki je nedavno prenehala delovati, je to morda zaradi tega, ker smo v okviru načrtov začeli [onemogočati šifro 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="347e1-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="347e1-105">Če si želite ogledati prizadete naprave, pojdite na[ Poročilo o odjemalcih s preverjanjem pristnosti SMTP Auth](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="347e1-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="347e1-106">Med pogostimi napakami so: napaka pri preverjanju pristnosti, napaka protokola TLS, napaka algoritma šifre, neujemanje algoritma ali prekinjena povezava.</span><span class="sxs-lookup"><span data-stu-id="347e1-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="347e1-107">Za odpravo težave:</span><span class="sxs-lookup"><span data-stu-id="347e1-107">To resolve the issue:</span></span>

 - <span data-ttu-id="347e1-108">**Sistem Windows Server 2003 IIS SMTP ne bo več deloval. Potrebujete novo različico sistema Windows.**</span><span class="sxs-lookup"><span data-stu-id="347e1-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="347e1-109">Pri dobavitelju aplikacije ali naprave preverite, ali je podprta sodobna šifra oz. ali je na voljo posodobitev.</span><span class="sxs-lookup"><span data-stu-id="347e1-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
