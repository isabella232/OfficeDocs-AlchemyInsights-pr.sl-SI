---
title: Odpravljanje težav z uvajanjem potrdila o pristnosti odjemalca
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659002"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="c7830-102">Odpravljanje težav z uvajanjem potrdila o pristnosti odjemalca</span><span class="sxs-lookup"><span data-stu-id="c7830-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="c7830-103">InTune NDES/SCEP in PKCS/PFX profili potrdil odjemalca se običajno uporabljajo v povezavi z drugimi vrstami profilov, kot so WiFi, VPN in e-pošta, da uporabnikom omogočijo preverjanje pristnosti za vire podjetja.</span><span class="sxs-lookup"><span data-stu-id="c7830-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="c7830-104">Ko so te vrste profilov povezane s profilom potrdila odjemalca, so odvisne od uspešne uvedbe tega profila.</span><span class="sxs-lookup"><span data-stu-id="c7830-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="c7830-105">Začetna nastavitev infrastrukture in povezana konfiguracija profila odjemalčevega potrdila pogosto zahtevata odpravljanje težav.</span><span class="sxs-lookup"><span data-stu-id="c7830-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="c7830-106">Če želite navodila po korakih za uspešno nastavitev povezovalnika NDES in navodila za odpravljanje težav pri izoliranju težav s uvajanjem potrdila, glejte:</span><span class="sxs-lookup"><span data-stu-id="c7830-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="c7830-107">Konfiguracija infrastrukture za podporo SCEP z InTune</span><span class="sxs-lookup"><span data-stu-id="c7830-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="c7830-108">Pregled za odpravljanje težav SCEP profilov potrdil z Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="c7830-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="c7830-109">Uporabite referenčne skripte PowerShell za pomoč pri preverjanju konfiguracije.</span><span class="sxs-lookup"><span data-stu-id="c7830-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="c7830-110">Če želite več informacij, glejte Iskanje [skriptov za preverjanje priključka potrdila](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="c7830-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="c7830-111">**Druge pogoste težave**</span><span class="sxs-lookup"><span data-stu-id="c7830-111">**Other common issues**</span></span>

<span data-ttu-id="c7830-112">**Ko poskusim namestiti povezovalnik» InTune «v strežniku NDES Connector, dobim sporočilo, da» gesla v zahtevi za potrdilo ni mogoče preveriti. Morda je bil že uporabljen. Pridobite novo geslo, ki ga želite poslati s to zahtevo. «**</span><span class="sxs-lookup"><span data-stu-id="c7830-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="c7830-113">To sporočilo pomeni, da morate zagnati namestitev povezovalnika potrdila kot skrbnik.</span><span class="sxs-lookup"><span data-stu-id="c7830-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="c7830-114">V nekaterih okoljih morajo strežniki, v katerih se izvaja potrdilo InTune, uporabljati proxy strežnik, s katerim lahko vzpostavite povezavo s funkcijo InTune, zato mora povezovalnik potrdil uporabiti proxy.</span><span class="sxs-lookup"><span data-stu-id="c7830-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="c7830-115">V nekaterih primerih povezovalnik NDES prezre konfigurirane nastavitve proxyja in bo morda treba konfigurirati nastavitve strežnika proxy, medtem ko se izvaja v varnostnem kontekstu LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="c7830-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="c7830-116">Rešitev je, da zaženete Internet Explorer kot sistem in konfigurirate proxy v IE.</span><span class="sxs-lookup"><span data-stu-id="c7830-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="c7830-117">Po vnovičnem zagonu storitve priključka za InTune se NDES povezovalnik poveže z InTune.</span><span class="sxs-lookup"><span data-stu-id="c7830-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="c7830-118">**Uporabniške naprave ne prejemajo več SCEP potrdil iz NDES.**</span><span class="sxs-lookup"><span data-stu-id="c7830-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="c7830-119">Možno je, da je potrdilo o pristnosti odjemalca, izdano v strežnik NDES, in določeno med namestitvijo povezovalnika NDES, poteklo ali manjka.</span><span class="sxs-lookup"><span data-stu-id="c7830-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="c7830-120">Če želite razrešiti:</span><span class="sxs-lookup"><span data-stu-id="c7830-120">To resolve:</span></span> 
 
1. <span data-ttu-id="c7830-121">Odstranite povezovalnik NDES.</span><span class="sxs-lookup"><span data-stu-id="c7830-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="c7830-122">S temi podrobnostmi lahko zahtevate novo preverjanje pristnosti odjemalca ali potrdilo za preverjanje pristnosti strežnika:</span><span class="sxs-lookup"><span data-stu-id="c7830-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="c7830-123">Ime zadeve: CN = zunanji FQDN</span><span class="sxs-lookup"><span data-stu-id="c7830-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="c7830-124">Ime nadomestnega predmeta (oba sta obvezna): DNS = zunanji FQDN, DNS = Internal FQDN</span><span class="sxs-lookup"><span data-stu-id="c7830-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="c7830-125">Znova namestite povezovalnik NDES z novim potrdilom.</span><span class="sxs-lookup"><span data-stu-id="c7830-125">Reinstall the NDES connector with the new certificate.</span></span>