---
title: Zaščita podatkov-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908725"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="bc84b-102">Omogočanje šifriranja BitLocker z InTune</span><span class="sxs-lookup"><span data-stu-id="bc84b-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="bc84b-103">Za konfiguriranje nastavitev šifriranja BitLocker za naprave s sistemom Windows lahko uporabite pravilnik o zaščiti končne točke.</span><span class="sxs-lookup"><span data-stu-id="bc84b-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="bc84b-104">Če želite več informacij, glejte [nastavitve sistema Windows 10 (in novejše) za zaščito naprav z InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="bc84b-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="bc84b-105">Zavedati se morate, da številne novejše naprave s sistemom Windows 10 podpirajo samodejno šifriranje BitLocker, ki se sproži brez uporabe pravilnika MDM.</span><span class="sxs-lookup"><span data-stu-id="bc84b-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="bc84b-106">To lahko vpliva na uporabo pravilnika, če so konfigurirane neprivzete nastavitve.</span><span class="sxs-lookup"><span data-stu-id="bc84b-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="bc84b-107">Za podrobnejše podrobnosti si oglejte ta pogosta vprašanja.</span><span class="sxs-lookup"><span data-stu-id="bc84b-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="bc84b-108">Če želite več informacij o odpravljanju težav s funkcijo BitLocker, glejte [Odpravljanje težav s pravilniki funkcije BitLocker v programu Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="bc84b-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="bc84b-109">**Faq**</span><span class="sxs-lookup"><span data-stu-id="bc84b-109">**FAQ**</span></span>

 <span data-ttu-id="bc84b-110">V: katere izdaje šifriranja naprave sistema Windows z uporabo pravilnika o zaščiti končnih točk?</span><span class="sxs-lookup"><span data-stu-id="bc84b-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="bc84b-111">O: nastavitve v pravilniku o zaščiti končne točke se izvajajo s programom [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="bc84b-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="bc84b-112">Program BitLocker CSP ne podpira vseh izdaj ali nadgradi sistema Windows.</span><span class="sxs-lookup"><span data-stu-id="bc84b-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="bc84b-113">V tem času so podprte naslednje izdaje sistema Windows: Enterprise, Education, Mobile, Mobile Enterprise in Professional (gradnja 1809 in novejše različice).</span><span class="sxs-lookup"><span data-stu-id="bc84b-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="bc84b-114">V: če je naprava že šifrirana s funkcijo BitLocker z uporabo privzetih nastavitev OS za način šifriranja in moč šifre (XTS-AES-128), bo uporaba pravilnika z različnimi nastavitvami samodejno sprožila ponovno šifriranje pogona z novimi nastavitvami?</span><span class="sxs-lookup"><span data-stu-id="bc84b-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="bc84b-115">A: ne.</span><span class="sxs-lookup"><span data-stu-id="bc84b-115">A: No.</span></span> <span data-ttu-id="bc84b-116">Če želite uporabiti nove nastavitve šifre, morate najprej dešifrirati pogon.</span><span class="sxs-lookup"><span data-stu-id="bc84b-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="bc84b-117">**Opomba:** Za naprave, ki se vpisujejo z avtopilot, se samodejno šifriranje, ki se pojavi med OOBE, ne sproži, dokler se ne ovrednoti pravilnik InTune, ki omogoča uporabo nastavitev pravilnika, ki se uporablja namesto privzetih vrednosti OPERACIJSKEGA sistema.</span><span class="sxs-lookup"><span data-stu-id="bc84b-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="bc84b-118">V: če je naprava šifrirana zaradi uporabe pravilnika InTune, ali bo dešifrirala, ko je ta pravilnik odstranjen?</span><span class="sxs-lookup"><span data-stu-id="bc84b-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="bc84b-119">O: odstranitev pravilnika, povezane s šifriranjem, ne povzroči dešifriranja pogonov, ki so bili konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="bc84b-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="bc84b-120">V: zakaj InTune pravilnik o skladnosti kaže, da moja naprava nima omogočenega pogona BitLocker, čeprav je?</span><span class="sxs-lookup"><span data-stu-id="bc84b-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="bc84b-121">O: nastavitev» BitLocker Enabled «v pravilniku o skladnosti s skladnostjo uporablja odjemalca za potrdilo o zdravstvenem stanju naprave Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="bc84b-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="bc84b-122">Ta odjemalec meri samo stanje naprave ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="bc84b-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="bc84b-123">Če naprava ni bila znova zagnana, ker je šifriranje BitLocker končano, odjemalska storitev DHA ne bo poročala, da je BitLocker aktiven.</span><span class="sxs-lookup"><span data-stu-id="bc84b-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 