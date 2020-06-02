---
title: 2681 Attack simulator v Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506754"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="56cea-102">Attack simulator v Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="56cea-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="56cea-103">Ali ste manjka Attack simulator?</span><span class="sxs-lookup"><span data-stu-id="56cea-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="56cea-104">Attack simulator zahteva **office 365 napredno zaščito pred grožnjami načrt 2 (ATP načrt 2)** ali **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="56cea-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="56cea-105">Attack simulator ni **vključen v** Office 365 napredno zaščito pred grožnjami načrt 1 (ATP plan 1), Office 365 Enterprise E3, ali katere koli Microsoftove 365 apps za poslovne naročnine.</span><span class="sxs-lookup"><span data-stu-id="56cea-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="56cea-106">Račun, ki ga uporabljate za zagon simuliranih napadov, zahteva globalne skrbniške ali varnostne skrbniške pravice in večfaktorsko preverjanje pristnosti (MFA).</span><span class="sxs-lookup"><span data-stu-id="56cea-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="56cea-107">Če želite več informacij o zahtevah za Attack simulator, si oglejte [to temo](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="56cea-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="56cea-108">Važen stvari znati približno **živalski moč parola** napad Simulations:</span><span class="sxs-lookup"><span data-stu-id="56cea-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="56cea-109">Če je ciljni račun omogočen MFA in je bilo geslo pravilno ugano, račun ne bo prikazan kot ogrožen (drugi faktor za preverjanje pristnosti bo nepopoln).</span><span class="sxs-lookup"><span data-stu-id="56cea-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="56cea-110">Datoteka z geslom ne more biti večja od 10 MB.</span><span class="sxs-lookup"><span data-stu-id="56cea-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="56cea-111">Uporabite eno geslo na vrstico in na seznamu vključite prazno črto (povratni prevoz).</span><span class="sxs-lookup"><span data-stu-id="56cea-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="56cea-112">Pomembne stvari vedeti o **kopje phishing** priložite simulacije:</span><span class="sxs-lookup"><span data-stu-id="56cea-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="56cea-113">Po zasnovi ne morete zagotoviti vrednosti po meri za **URL strežnika za prijavo lažnega predstavljanja**.</span><span class="sxs-lookup"><span data-stu-id="56cea-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="56cea-114">Če prejemnik uporabi možnost [Omogoči dodajanje sporočila poročila](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , da sporočilo sporoči kot lažno predstavljanje, morda ne boste prejeli opozoril za sporočilo (ker je to simuliran napad).</span><span class="sxs-lookup"><span data-stu-id="56cea-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="56cea-115">Poročila: ko je simuliran napad končan, lahko kliknete **napad podrobnosti** , da si ogledate poročilo.</span><span class="sxs-lookup"><span data-stu-id="56cea-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="56cea-116">Za podrobna navodila in nove funkcije v Attack simulator, glej [Attack simulator v Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="56cea-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
