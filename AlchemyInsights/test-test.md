---
title: Pogoji, ki jih ni v trgovini SharePoint online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750467"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="b6545-102">Omogočanje šifriranja BitLockerja s funkcijo InTune</span><span class="sxs-lookup"><span data-stu-id="b6545-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="b6545-103">Če želite konfigurirati nastavitve šifriranja Boitlocker za naprave s sistemom Windows, kot je opisano v: Windows10 (in novejših), uporabite nastavitve za zaščito naprav s funkcijo InTune</span><span class="sxs-lookup"><span data-stu-id="b6545-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="b6545-104">Zavedati se morate, da številne novejše naprave, v katerih je nameščen Windows 10, podpirajo samodejno šifriranje BitLockerja, ki se sproži brez uporabe pravilnika MDM.</span><span class="sxs-lookup"><span data-stu-id="b6545-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="b6545-105">To lahko vpliva na uporabo pravilnika, če niso privzete nastavitve konfigurirane.</span><span class="sxs-lookup"><span data-stu-id="b6545-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="b6545-106">Če želite več podrobnosti, glejte Pogosta vprašanja.</span><span class="sxs-lookup"><span data-stu-id="b6545-106">See FAQ for more detail.</span></span>


<span data-ttu-id="b6545-107">Pogosta vprašanja   o tem: katere izdaje šifriranja naprave za Windows podpirajo s pravilnikom o zaščiti končnih točk?</span><span class="sxs-lookup"><span data-stu-id="b6545-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="b6545-108"> A: nastavitve v pravilniku o zaščiti končnih točk se izvajajo s sistemom BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="b6545-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="b6545-109">Ni vseh izdaj in ne gradi sistema Windows, ki podpirajo sistem BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="b6545-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="b6545-110">V tem času izdaje sistema Windows: Enterprise; Podpora za izobraževanje, mobilno, mobilno podjetništvo in Professional (od gradnje 1809 naprej).</span><span class="sxs-lookup"><span data-stu-id="b6545-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="b6545-111">V: če je naprava že šifrirana s funkcijo BitLocker s privzetimi nastavitvami sistema OS za način šifriranja in trdnost ključa (XTS-AES-128), bo uporaba pravilnika z različnimi nastavitvami samodejno sprožil vnovično šifriranje pogona z novimi nastavitvami?</span><span class="sxs-lookup"><span data-stu-id="b6545-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="b6545-112">O: Ne.</span><span class="sxs-lookup"><span data-stu-id="b6545-112">A: No.</span></span> <span data-ttu-id="b6545-113">Če želite uporabiti nove nastavitve šifer, mora biti pogon najprej dešifriran.</span><span class="sxs-lookup"><span data-stu-id="b6545-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="b6545-114">Opomba pri napravah, ki so vpisani s samodejnim avtopilotom, se samodejno šifriranje, ki se pojavi med OOBE, ne sproži, dokler ni ovrednoten pravilnik, ki omogoča uporabo nastavitev pravilnika, ki jih je treba uporabiti namesto privzetih vrednosti za OS.</span><span class="sxs-lookup"><span data-stu-id="b6545-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="b6545-115">Q Če je naprava šifrirana zaradi uporabe pravilnika za InTune, bo dešifrirana, ko je ta pravilnik odstranjen?</span><span class="sxs-lookup"><span data-stu-id="b6545-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="b6545-116">A: odstranitev pravilnika, povezanega s šifriranjem, ne povzroči dešifriranja pogonov, ki so bili konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="b6545-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="b6545-117">V: zakaj pravilnik o skladnosti s predpisi pokaže, da moja naprava nima omogočene funkcije» BitLocker «;</span><span class="sxs-lookup"><span data-stu-id="b6545-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="b6545-118">A: nastavitev» BitLocker Enabled «v pravilniku o skladnosti s predpisi, ki uporablja odjemalca s sistemom Windows za zdravstveno varstvo (DHA).</span><span class="sxs-lookup"><span data-stu-id="b6545-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="b6545-119">Ta odjemalec samo določi stanje naprave ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="b6545-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="b6545-120">Če naprava ni bila znova zagnana, ker je bilo šifriranje BitLocker dokončano, odjemalska storitev DHA ne bo prijavila funkcije BitLocker kot aktivno.</span><span class="sxs-lookup"><span data-stu-id="b6545-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>