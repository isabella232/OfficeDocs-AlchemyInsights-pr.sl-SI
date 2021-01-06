---
title: DataProtection – BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768833"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="e96be-102">Omogočanje šifriranja BitLockerja s funkcijo InTune</span><span class="sxs-lookup"><span data-stu-id="e96be-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="e96be-103">Če želite konfigurirati nastavitve šifriranja BitLockerja za naprave s sistemom Windows, lahko nastavite pravilnik o zaščiti končnih točk.</span><span class="sxs-lookup"><span data-stu-id="e96be-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="e96be-104">Če želite več informacij, glejte [nastavitve sistema Windows 10 (in novejše različice) za zaščito naprav s funkcijo InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="e96be-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="e96be-105">Zavedati se morate, da številne novejše naprave, v katerih je nameščen Windows 10, podpirajo samodejno šifriranje BitLockerja, ki se sproži brez uporabe pravilnika MDM.</span><span class="sxs-lookup"><span data-stu-id="e96be-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="e96be-106">To lahko vpliva na uporabo pravilnika, če so konfigurirane privzete nastavitve.</span><span class="sxs-lookup"><span data-stu-id="e96be-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="e96be-107">Če želite več podrobnosti, si oglejte ta pogosta vprašanja.</span><span class="sxs-lookup"><span data-stu-id="e96be-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="e96be-108">Če želite več informacij o odpravljanju težav z BitLockerjem, glejte [Odpravljanje težav s pravilniki BitLockerja v programu Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="e96be-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="e96be-109">**Pogosta vprašanja**</span><span class="sxs-lookup"><span data-stu-id="e96be-109">**FAQ**</span></span>

<span data-ttu-id="e96be-110">V: katere izdaje šifriranja naprave s sistemom Windows s pravilnikom o zaščiti končnih točk?</span><span class="sxs-lookup"><span data-stu-id="e96be-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="e96be-111">A: nastavitve v pravilniku o zaščiti končnih točk se izvajajo s sistemom [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="e96be-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="e96be-112">Niso vse izdaje ali gradi sistema Windows, ki podpirajo sistem BitLocker.</span><span class="sxs-lookup"><span data-stu-id="e96be-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="e96be-113">V: kako je mogoče omogočiti BitLocker v napravah, ne da bi to zahtevalo dostop do končnega uporabnika?</span><span class="sxs-lookup"><span data-stu-id="e96be-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="e96be-114">A: dokler so izpolnjeni potrebni predpogoji, je mogoče omogočiti BitLocker» Silent encryption «s funkcijo InTune.</span><span class="sxs-lookup"><span data-stu-id="e96be-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="e96be-115">Oglejte si podrobnosti o zahtevah za napravo in primer nastavitev pravilnika za omogočanje tihega šifriranja v tem dokumentu: [tiho omogočanje šifriranja BitLockerja](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="e96be-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="e96be-116">V: če je naprava že šifrirana s funkcijo BitLocker s privzetimi nastavitvami sistema OS za način šifriranja in trdnost ključa (XTS-AES-128), bo uporaba pravilnika z različnimi nastavitvami samodejno sprožil vnovično šifriranje pogona z novimi nastavitvami?</span><span class="sxs-lookup"><span data-stu-id="e96be-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="e96be-117">O: Ne.</span><span class="sxs-lookup"><span data-stu-id="e96be-117">A: No.</span></span> <span data-ttu-id="e96be-118">Če želite uporabiti nove nastavitve šifer, mora biti pogon najprej dešifriran.</span><span class="sxs-lookup"><span data-stu-id="e96be-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="e96be-119">**Opomba:** Za naprave, ki so vpisane s samodejnim pilotom, se samodejno šifriranje, ki se pojavi med OOBE, ne sproži, dokler ni ovrednoten pravilnik, ki omogoča uporabo nastavitev pravilnika, ki jih je treba uporabiti namesto privzetih vrednosti za OS.</span><span class="sxs-lookup"><span data-stu-id="e96be-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="e96be-120">V: če je naprava šifrirana zaradi uporabe pravilnika za InTune, bo dešifrirana, ko je ta pravilnik odstranjen?</span><span class="sxs-lookup"><span data-stu-id="e96be-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="e96be-121">A: odstranitev pravilnika, povezanega s šifriranjem, ne povzroči dešifriranja pogonov, ki so bili konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="e96be-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="e96be-122">V: zakaj pravilnik o skladnosti s predpisi pokaže, da moja naprava nima omogočenega pogona BitLocker, čeprav je?</span><span class="sxs-lookup"><span data-stu-id="e96be-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="e96be-123">A: nastavitev» BitLocker Enabled «v pravilniku o skladnosti s predpisi uporablja odjemalca za potrdilo o zdravstvenem stanju sistema Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="e96be-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="e96be-124">Ta odjemalec samo določi stanje naprave ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="e96be-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="e96be-125">Če naprava ni bila znova zagnana, ker je bila šifrirana BitLocker dokončana, odjemalska storitev DHA ne bo prijavila funkcije BitLocker kot aktivno.</span><span class="sxs-lookup"><span data-stu-id="e96be-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 