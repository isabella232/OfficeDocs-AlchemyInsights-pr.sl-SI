---
title: Odpravljanje težav pri uvajanju potrdila za preverjanje pristnosti odjemalca
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555809"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="023a5-102">Odpravljanje težav pri uvajanju potrdila za preverjanje pristnosti odjemalca</span><span class="sxs-lookup"><span data-stu-id="023a5-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="023a5-103">Profili certifikatov NDES/SCEP in PKCS/PFX client se običajno uporabljajo v povezavi z drugimi vrstami profilov, kot so Wifi, VPN in e-pošta, ki uporabnikom omogočajo preverjanje pristnosti s poslovnimi viri.</span><span class="sxs-lookup"><span data-stu-id="023a5-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="023a5-104">Če so te vrste profilov povezane s profilom potrdila odjemalca, so odvisne od uspešne uvedbe tega profila.</span><span class="sxs-lookup"><span data-stu-id="023a5-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="023a5-105">Začetna nastavitev infrastrukture in povezana konfiguracija profila odjemalskega potrdila pogosto zahtevata odpravljanje težav.</span><span class="sxs-lookup"><span data-stu-id="023a5-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="023a5-106">Navodila za uspešno namestitev konektorja NDES in navodila za odpravljanje težav za izolacijo težav pri uvajanju certifikatov so na voljo v navodilih za odpravljanje težav, glejte:</span><span class="sxs-lookup"><span data-stu-id="023a5-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="023a5-107">Konfiguracija infrastrukture za podporo SCEP z Intune</span><span class="sxs-lookup"><span data-stu-id="023a5-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="023a5-108">Pregled za odpravljanje težav s certifikatnimi profili SCEP z MicrosoftOm Intune</span><span class="sxs-lookup"><span data-stu-id="023a5-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="023a5-109">S skripti powershell, na katere se sklicujete, lahko preverite konfiguracijo.</span><span class="sxs-lookup"><span data-stu-id="023a5-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="023a5-110">Če želite več informacij, [glejte Skripti za preverjanje potrdila intune .](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)</span><span class="sxs-lookup"><span data-stu-id="023a5-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="023a5-111">**Druga pogosta vprašanja**</span><span class="sxs-lookup"><span data-stu-id="023a5-111">**Other common issues**</span></span>

<span data-ttu-id="023a5-112">**Ko poskušam namestiti konektor potrdila Intune na strežniku konektorja NDES, se prikaže sporočilo »Gesla v zahtevi za potrdilo ni mogoče preveriti. Morda je že bil uporabljen. Pridobite novo geslo za pošiljanje s to zahtevo."**</span><span class="sxs-lookup"><span data-stu-id="023a5-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="023a5-113">To sporočilo pomeni, da morate namestitev certifikatnega konektorja zagnati kot skrbnika.</span><span class="sxs-lookup"><span data-stu-id="023a5-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="023a5-114">V nekaterih okoljih morajo strežniki, v katerih se izvaja potrdilo Intune, za povezavo z intunom uporabiti proxy strežnik, zato mora certifikatni konektor uporabljati proxy.</span><span class="sxs-lookup"><span data-stu-id="023a5-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="023a5-115">V nekaterih okoliščinah NDES Connector prezre konfigurirane nastavitve strežnika proxy in morda bo treba konfigurirati nastavitve strežnika proxy med izvajanjem v varnostnem kontekstu lokalnega sistema.</span><span class="sxs-lookup"><span data-stu-id="023a5-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="023a5-116">Rešitev je, da zaženete Internet Explorer kot SYSTEM in konfigurirate proxy v IE.</span><span class="sxs-lookup"><span data-stu-id="023a5-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="023a5-117">Po vnovičnem zagonu storitve intune connector se konektor NDES poveže z intunom.</span><span class="sxs-lookup"><span data-stu-id="023a5-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="023a5-118">**Uporabniške naprave ne prejemajo več certifikatov SCEP od NDES-a.**</span><span class="sxs-lookup"><span data-stu-id="023a5-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="023a5-119">Možno je, da je potrdilo za preverjanje pristnosti odjemalca, izdano strežniku NDES in je določeno med namestitvijo konektorja NDES, poteklo ali manjka.</span><span class="sxs-lookup"><span data-stu-id="023a5-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="023a5-120">Če želite odpraviti:</span><span class="sxs-lookup"><span data-stu-id="023a5-120">To resolve:</span></span> 
 
1. <span data-ttu-id="023a5-121">Odstranite konektor NDES.</span><span class="sxs-lookup"><span data-stu-id="023a5-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="023a5-122">Te podrobnosti uporabite, če želite zahtevati novo preverjanje pristnosti odjemalca ali potrdilo za preverjanje pristnosti strežnika:</span><span class="sxs-lookup"><span data-stu-id="023a5-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="023a5-123">Ime zadeve: CN=zunanji fqdn</span><span class="sxs-lookup"><span data-stu-id="023a5-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="023a5-124">Nadomestno ime zadeve (oba sta potrebna): DNS=zunanji fqdn, DNS=notranji fqdn</span><span class="sxs-lookup"><span data-stu-id="023a5-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="023a5-125">Znova namestite konektor NDES z novim potrdilom.</span><span class="sxs-lookup"><span data-stu-id="023a5-125">Reinstall the NDES connector with the new certificate.</span></span>