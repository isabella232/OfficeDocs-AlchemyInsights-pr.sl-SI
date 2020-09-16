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
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731255"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="6dab6-102">Omogočanje šifriranja BitLockerja s funkcijo InTune</span><span class="sxs-lookup"><span data-stu-id="6dab6-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="6dab6-103">Če želite konfigurirati nastavitve šifriranja BitLockerja za naprave s sistemom Windows, lahko nastavite pravilnik o zaščiti končnih točk.</span><span class="sxs-lookup"><span data-stu-id="6dab6-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="6dab6-104">Če želite več informacij, glejte [nastavitve sistema Windows 10 (in novejše različice) za zaščito naprav s funkcijo InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="6dab6-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="6dab6-105">Zavedati se morate, da številne novejše naprave, v katerih je nameščen Windows 10, podpirajo samodejno šifriranje BitLockerja, ki se sproži brez uporabe pravilnika MDM.</span><span class="sxs-lookup"><span data-stu-id="6dab6-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="6dab6-106">To lahko vpliva na uporabo pravilnika, če so konfigurirane privzete nastavitve.</span><span class="sxs-lookup"><span data-stu-id="6dab6-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="6dab6-107">Če želite več podrobnosti, si oglejte ta pogosta vprašanja.</span><span class="sxs-lookup"><span data-stu-id="6dab6-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="6dab6-108">Če želite več informacij o odpravljanju težav z BitLockerjem, glejte [Odpravljanje težav s pravilniki BitLockerja v programu Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="6dab6-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="6dab6-109">**Pogosta vprašanja**</span><span class="sxs-lookup"><span data-stu-id="6dab6-109">**FAQ**</span></span>

 <span data-ttu-id="6dab6-110">V: katere izdaje šifriranja naprave s sistemom Windows s pravilnikom o zaščiti končnih točk?</span><span class="sxs-lookup"><span data-stu-id="6dab6-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="6dab6-111">A: nastavitve v pravilniku o zaščiti končnih točk se izvajajo s sistemom [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="6dab6-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="6dab6-112">Niso vse izdaje ali gradi sistema Windows, ki podpirajo sistem BitLocker.</span><span class="sxs-lookup"><span data-stu-id="6dab6-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="6dab6-113">V tem trenutku so podprte te izdaje sistema Windows: Enterprise, Education, Mobile, Mobile Enterprise in Professional (graditev 1809 in novejša različica).</span><span class="sxs-lookup"><span data-stu-id="6dab6-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="6dab6-114">V: če je naprava že šifrirana s funkcijo BitLocker s privzetimi nastavitvami sistema OS za način šifriranja in trdnost ključa (XTS-AES-128), bo uporaba pravilnika z različnimi nastavitvami samodejno sprožil vnovično šifriranje pogona z novimi nastavitvami?</span><span class="sxs-lookup"><span data-stu-id="6dab6-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="6dab6-115">O: Ne.</span><span class="sxs-lookup"><span data-stu-id="6dab6-115">A: No.</span></span> <span data-ttu-id="6dab6-116">Če želite uporabiti nove nastavitve šifer, mora biti pogon najprej dešifriran.</span><span class="sxs-lookup"><span data-stu-id="6dab6-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="6dab6-117">**Opomba:** Za naprave, ki so vpisane s samodejnim pilotom, se samodejno šifriranje, ki se pojavi med OOBE, ne sproži, dokler ni ovrednoten pravilnik, ki omogoča uporabo nastavitev pravilnika, ki jih je treba uporabiti namesto privzetih vrednosti za OS.</span><span class="sxs-lookup"><span data-stu-id="6dab6-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="6dab6-118">V: če je naprava šifrirana zaradi uporabe pravilnika za InTune, bo dešifrirana, ko je ta pravilnik odstranjen?</span><span class="sxs-lookup"><span data-stu-id="6dab6-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="6dab6-119">A: odstranitev pravilnika, povezanega s šifriranjem, ne povzroči dešifriranja pogonov, ki so bili konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="6dab6-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="6dab6-120">V: zakaj pravilnik o skladnosti s predpisi pokaže, da moja naprava nima omogočenega pogona BitLocker, čeprav je?</span><span class="sxs-lookup"><span data-stu-id="6dab6-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="6dab6-121">A: nastavitev» BitLocker Enabled «v pravilniku o skladnosti s predpisi uporablja odjemalca za potrdilo o zdravstvenem stanju sistema Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="6dab6-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="6dab6-122">Ta odjemalec samo določi stanje naprave ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="6dab6-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="6dab6-123">Če naprava ni bila znova zagnana, ker je bila šifrirana BitLocker dokončana, odjemalska storitev DHA ne bo prijavila funkcije BitLocker kot aktivno.</span><span class="sxs-lookup"><span data-stu-id="6dab6-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 