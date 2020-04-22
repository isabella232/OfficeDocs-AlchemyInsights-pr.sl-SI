---
title: Manjkajoči pogoji iz trgovine SharePoint online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766869"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="3ae96-102">Omogočanje šifriranja BitLocker z InTune</span><span class="sxs-lookup"><span data-stu-id="3ae96-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="3ae96-103">Za konfiguriranje nastavitev šifriranja Boitlocker za naprave s sistemom Windows, kot je opisano v temi: Windows10 (in novejše) nastavitve za zaščito naprav z InTune, je mogoče uporabiti pravilnik o zaščiti končne točke.</span><span class="sxs-lookup"><span data-stu-id="3ae96-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="3ae96-104">Zavedati se morate, da številne novejše naprave s sistemom Windows 10 podpirajo samodejno šifriranje BitLocker, ki se sproži brez uporabe pravilnika MDM.</span><span class="sxs-lookup"><span data-stu-id="3ae96-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="3ae96-105">To lahko vpliva na uporabo pravilnika, če niso konfigurirane privzete nastavitve.</span><span class="sxs-lookup"><span data-stu-id="3ae96-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="3ae96-106">Za podrobnejše podrobnosti glejte Pogosta vprašanja.</span><span class="sxs-lookup"><span data-stu-id="3ae96-106">See FAQ for more detail.</span></span>


<span data-ttu-id="3ae96-107">Pogosta  vprašanja Q: katere izdaje šifriranja naprave s sistemom Windows s pravilnikom o zaščiti končne točke?</span><span class="sxs-lookup"><span data-stu-id="3ae96-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="3ae96-108"> O: nastavitve v pravilniku o zaščiti končne točke se izvajajo s programom BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="3ae96-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="3ae96-109">BitLocker CSP ne podpira vseh izdaj niti ne gradi sistema Windows. 
     </span><span class="sxs-lookup"><span data-stu-id="3ae96-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="3ae96-110">V tem času Windows Editions: Enterprise; Izobraževanje, Mobile, Mobile Enterprise in Professional (od izgradnje 1809 naprej) so podprte.</span><span class="sxs-lookup"><span data-stu-id="3ae96-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="3ae96-111">V: če je naprava že šifrirana s funkcijo BitLocker z uporabo privzetih nastavitev OS za način šifriranja in moč šifre (XTS-AES-128) bo uporabil pravilnik z različnimi nastavitvami samodejno sproži ponovno šifriranje pogona z novimi nastavitvami?</span><span class="sxs-lookup"><span data-stu-id="3ae96-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="3ae96-112">A: ne.</span><span class="sxs-lookup"><span data-stu-id="3ae96-112">A: No.</span></span> <span data-ttu-id="3ae96-113">Da bi uporabili nove nastavitve šifre, morate pogon najprej dešifrirati.</span><span class="sxs-lookup"><span data-stu-id="3ae96-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="3ae96-114">Opomba za naprave, ki se vpisujejo z avtopilot, se samodejno šifriranje, ki se pojavi med OOBE, ne sproži, dokler se ne ovrednoti pravilnik InTune, ki omogoča uporabo nastavitev pravilnika, ki se uporablja namesto privzetih vrednosti OPERACIJSKEGA sistema</span><span class="sxs-lookup"><span data-stu-id="3ae96-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="3ae96-115">Q Če je naprava šifrirana zaradi uporabe pravilnika InTune bo dešifrirati, ko je ta pravilnik odstranjen?</span><span class="sxs-lookup"><span data-stu-id="3ae96-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="3ae96-116">O: odstranitev pravilnika, povezane s šifriranjem, ne povzroči dešifriranje pogonov, ki so bili konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="3ae96-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="3ae96-117">V: zakaj InTune pravilnik o skladnosti kaže, da moja naprava nima "BitLocker Enabled", vendar je?</span><span class="sxs-lookup"><span data-stu-id="3ae96-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="3ae96-118">O: nastavitev» BitLocker Enabled «v pravilniku o izpolnjevanju pravil skladnosti uporablja odjemalca za potrdilo o zdravstvenem stanju naprave Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="3ae96-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="3ae96-119">Ta odjemalec meri samo stanje naprave ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="3ae96-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="3ae96-120">Torej, če naprava ni bila znova zagnana, ker je šifriranje BitLocker končano, odjemalska storitev DHA ne bo poročala, da je BitLocker aktiven.</span><span class="sxs-lookup"><span data-stu-id="3ae96-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>