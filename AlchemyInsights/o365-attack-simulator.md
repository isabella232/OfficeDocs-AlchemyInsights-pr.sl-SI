---
title: 2681 Attack Rio in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545742"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="cd079-102">Attack Rio in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="cd079-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="cd079-103">Ali pogrešate napadajoče napade?</span><span class="sxs-lookup"><span data-stu-id="cd079-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="cd079-104">Plan **2 ali Office 365 (Paket 2)** ali **paket Office 365 Enterprise E5** zahteva Microsoft Defender .</span><span class="sxs-lookup"><span data-stu-id="cd079-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="cd079-105">Storitev Attack Premium **ni vključena** v Microsoft Defender za Office 365 paket 1, Office 365 Enterprise E3 ali katere koli Programi Microsoft 365 za manjša podjetja naročnine.</span><span class="sxs-lookup"><span data-stu-id="cd079-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="cd079-106">Račun, ki ga uporabljate za zagon simuliranih napadov, zahteva dovoljenja globalnega skrbnika ali skrbnika za varnost in večkratno preverjanje pristnosti (MFA).</span><span class="sxs-lookup"><span data-stu-id="cd079-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="cd079-107">Če želite več informacij o zahtevah napadov z napadom, si [oglejte to temo.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="cd079-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="cd079-108">Pomembne stvari, ki jih je treba vedeti **o simulacijah napadov z** grobih geslih:</span><span class="sxs-lookup"><span data-stu-id="cd079-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="cd079-109">Če je v ciljnem računu omogočena storitev MFA in je bilo pravilno ugibanje gesla, račun ne bo prikazan kot ogrožen (drugi dejavnik preverjanja pristnosti bo nepopoln).</span><span class="sxs-lookup"><span data-stu-id="cd079-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="cd079-110">Datoteka z geslom ne sme biti večja od 10 MB.</span><span class="sxs-lookup"><span data-stu-id="cd079-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="cd079-111">Uporabite eno geslo na vrstico in vključite prazno vrstico (prelom vrstice) za zadnjim geslom na seznamu.</span><span class="sxs-lookup"><span data-stu-id="cd079-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="cd079-112">Pomembne stvari, ki jih je treba vedeti **o simulacijah prilaganja spearnega** lažnega predstavljanja:</span><span class="sxs-lookup"><span data-stu-id="cd079-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="cd079-113">Privzeto ni mogoče vati vrednosti po meri za URL strežnika za prijavo v lažno **predstavljanje.**</span><span class="sxs-lookup"><span data-stu-id="cd079-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="cd079-114">Če prejemnik uporablja dodatek Omogoči sporočilo poročila [za](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) prijavite sporočilo kot lažno, morda ne boste prejeli opozoril za sporočilo (ker gre za simuliran napad).</span><span class="sxs-lookup"><span data-stu-id="cd079-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="cd079-115">Poročila: Ko je simulacija napada končana, lahko kliknete **Podrobnosti** o napadu, da si ogledate poročilo.</span><span class="sxs-lookup"><span data-stu-id="cd079-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="cd079-116">Če želite podrobna navodila in nove funkcije v napadu Rio, glejte [Attack Rio v Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="cd079-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
