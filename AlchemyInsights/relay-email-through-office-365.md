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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117999"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="b3f43-102">Nastavite večfunkcijsko napravo ali aplikacijo za pošiljanje e-pošte</span><span class="sxs-lookup"><span data-stu-id="b3f43-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="b3f43-103">Več informacij o možnostih in navodila najdete v članku [Nastavitev večfunkcijske naprave ali aplikacije za pošiljanje e-pošte z okoljem Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="b3f43-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="b3f43-104">Če imate napravo ali aplikacijo, ki je nedavno prenehala delovati, so najpogostejše težave:</span><span class="sxs-lookup"><span data-stu-id="b3f43-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="b3f43-105">**Napake, povezane s preverjanjem pristnosti pri uporabi pošiljanja SMTP Auth odjemalca** Nedavno smo naredili nekaj sprememb, povezanih z načinom dela preverjanja pristnosti SMTP.</span><span class="sxs-lookup"><span data-stu-id="b3f43-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="b3f43-106">Če želite več informacij o odpravljanju težav, glejte razdelek o neuspešnem preverjanju pristnosti v razdelku Odpravljanje težav s tiskalniki, optičnimi bralniki in programi LOB, ki pošiljajo e-pošto s programom [Microsoft 365 ali Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)</span><span class="sxs-lookup"><span data-stu-id="b3f43-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="b3f43-107">**Sprejemamo le različico TLS 1.2, medtem ko pripravljamo varno povezavo za Office 365** Če uporabljate varno povezavo (TLS), se prepričajte, da vaša naprava aplikacije podpira TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="b3f43-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="b3f43-108">Če želite več informacij, [glejte Priprava na TLS 1.2](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)v Office 365 in Office 365 GCC.</span><span class="sxs-lookup"><span data-stu-id="b3f43-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="b3f43-109">Če želite druge težave in rešitve, glejte Odpravljanje težav s tiskalniki, optičnimi bralniki in aplikacijami LOB, ki pošiljajo e-pošto [s Microsoft 365 ali s Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)</span><span class="sxs-lookup"><span data-stu-id="b3f43-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="b3f43-110">Če si želite ogledati prizadete naprave, pojdite na[ Poročilo o odjemalcih s preverjanjem pristnosti SMTP Auth](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="b3f43-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="b3f43-111">**Opomba:** Exchange Online primeri množične pošte niso na voljo.</span><span class="sxs-lookup"><span data-stu-id="b3f43-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="b3f43-112">Če želite poslati množično komercialno e-pošto (na primer glasila strank), uporabite tretje ponudnike, ki so posebni za te storitve.</span><span class="sxs-lookup"><span data-stu-id="b3f43-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
