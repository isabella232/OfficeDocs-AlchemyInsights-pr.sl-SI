---
title: Posredovanje e-pošte prek okolja Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023475"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="15014-102">Nastavite večfunkcijsko napravo ali aplikacijo za pošiljanje e-pošte</span><span class="sxs-lookup"><span data-stu-id="15014-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="15014-103">Več informacij o možnostih in navodila najdete v članku [Nastavitev večfunkcijske naprave ali aplikacije za pošiljanje e-pošte z okoljem Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="15014-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="15014-104">**Opomba:** če imate napravo ali aplikacijo, ki je nedavno prenehala delovati, je to morda zaradi tega, ker smo v okviru načrtov začeli [onemogočati šifro 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="15014-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="15014-105">Če si želite ogledati prizadete naprave, pojdite na[ Poročilo o odjemalcih s preverjanjem pristnosti SMTP Auth](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="15014-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="15014-106">Med pogostimi napakami so: napaka pri preverjanju pristnosti, napaka protokola TLS, napaka algoritma šifre, neujemanje algoritma ali prekinjena povezava.</span><span class="sxs-lookup"><span data-stu-id="15014-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="15014-107">Za odpravo težave:</span><span class="sxs-lookup"><span data-stu-id="15014-107">To resolve the issue:</span></span>

 - <span data-ttu-id="15014-108">**Sistem Windows Server 2003 IIS SMTP ne bo več deloval. Potrebujete novo različico sistema Windows.**</span><span class="sxs-lookup"><span data-stu-id="15014-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="15014-109">Pri dobavitelju aplikacije ali naprave preverite, ali je podprta sodobna šifra oz. ali je na voljo posodobitev.</span><span class="sxs-lookup"><span data-stu-id="15014-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
