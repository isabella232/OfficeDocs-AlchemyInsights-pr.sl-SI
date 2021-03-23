---
title: Pogojni dostop blokiram z napravo, ki se je priključila domeni
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038103"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="2d8e0-102">Pogojni dostop blokiram z napravo, ki se je priključila domeni</span><span class="sxs-lookup"><span data-stu-id="2d8e0-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="2d8e0-103">**Zelo priporočljiva orodja**</span><span class="sxs-lookup"><span data-stu-id="2d8e0-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="2d8e0-104">[Orodje za odpravljanje težav z registracijo naprave](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – orodje, ki pomaga pri odpravljanju težav najpogostejše težave pri registraciji naprave.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="2d8e0-105">[Preskus povezljivosti za registracijo naprave](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – skript, ki pomaga zagotoviti, da lahko naprava dostopa do končnih točk za registracijo naprave v sistemskem računu.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="2d8e0-106">[Skript za čiščenje naprave AZURE ad](https://github.com/mzmaili/AzureADDeviceCleanup) – skript, ki omogoča iskanje in upravljanje zastarelih naprav v okolju.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="2d8e0-107">Tukaj je nekaj pogostih razlogov, zakaj pogojni dostop morda ne deluje v napravi, ki se je priključila domeni (hibridni Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2d8e0-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="2d8e0-108">V **napravi ni na voljo noben oglas Azure ad prt** – morate zagotoviti, da ima naprava primarni žeton za osveževanje v storitvi Azure ad (PRT).</span><span class="sxs-lookup"><span data-stu-id="2d8e0-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="2d8e0-109">Če želite več informacij o PRT, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="2d8e0-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="2d8e0-110">Če želite preveriti, ali imate v računalniku Azure AD PRT, lahko zaženete `dsregcmd/status` ukaz v napravi in preverite, ali je» AzureAdPrt «enako» da «.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="2d8e0-111">Če je» AzureAdPrt «» ne «, preverite to:</span><span class="sxs-lookup"><span data-stu-id="2d8e0-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="2d8e0-112">**Ne glede na to, ali imate Združeno okolje z AD FS in je nedosegljivo iz domačih omrežij uporabnikov**: v tem primeru zagotovite, da so končne točke» usernamemixed «dostopne iz Ekstranet.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="2d8e0-113">Če je vaš AD FS za VPN, zagotovite, da se uporabniki povežejo z VPN in se znova prijavijo v napravo.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="2d8e0-114">Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="2d8e0-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="2d8e0-115">**Ne glede na to, ali je modul zaupanja TPM okvarjen in s tem ne morete preveriti pristnosti naprave**: potrdite polje» TPM. msc «, da preverite, ali je stanje modula zaupanja TPM» Ready «.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="2d8e0-116">Če ne, zaženite `dsregcmd/leave` in pustite, da se naprava znova poveže s storitvijo AZURE ad.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="2d8e0-117">Nato poskusite znova.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-117">Then, try again.</span></span> <span data-ttu-id="2d8e0-118">Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="2d8e0-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="2d8e0-119">**Uporabljate ponudnika identitete tretje osebe, ki ne podpira WS-Trust protokola**.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="2d8e0-120">Kot je opisano v naših dokumentih, v tem primeru ne morejo delati hibridne naprave, ki so jih priključili v storitvi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="2d8e0-121">S ponudnikom identitete se obrnite na podporo.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="2d8e0-122">**Uporabniki uporabljajo brskalnik Chrome brez računov Windows 10** ali sistema **Office Extension Chrome ne uporablja samodejnega** dostopa do naprav, ki so na voljo s funkcijo» neregistrirano «ali s hibridno zvočno povezavo: to privede do neuspeha vseh pravilnikov o pogojnem dostopu, ki temeljijo na napravi, in prikaže se sporočilo o napaki» Neregistrirana naprava «.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="2d8e0-123">Če želite uporabiti brskalnik Chrome pravilno, morate namestiti» račune sistema Windows 10 «ali» razširitev sistema Office v brskalnik Chrome za uporabnike «prek SCCM ali InTune.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="2d8e0-124">Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="2d8e0-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="2d8e0-125">Če ne morete poriniti razširitve na daljavo, obvestite uporabnike, naj ročno namestite eno od zgornjih razširitev za dostop do programov za pogojni dostop, ki temelji na napravi.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="2d8e0-126">Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="2d8e0-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="2d8e0-127">**Naprava je bila pravilno hibridna AZURE ad JOIN, vendar je bila nehote izbrisana ali onemogočena, bodisi zaradi sprememb sinhronizacije v storitvi AZURE ad Connect ali iz portala Azure**: Če se to zgodi, se predmet naprave ne prepozna več kot popolnoma spojena naprava, čeprav je stanje» AzureAdJoined «in» prt «prikazano kot veljavno v napravi.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="2d8e0-128">Če želite odpraviti to težavo, zaženite v `dsregcmd/leave` prizadetih napravah in jim dovolite, da se znova vključijo v AZURE ad.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="2d8e0-129">Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="2d8e0-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="2d8e0-130">Če so vaše naprave na voljo v sistemu Windows 10, 1809 Update z VPN/Cloud proxy in si ogledate težave s stanjem» AzureAdPrt «ali katero koli aplikacijo s težavo SSO (Outlook se ne poveže z nabiralnikom, čeprav ste imeli PRT), zagotovite, da imate to popravek [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ali aprilski kumulativni posodobitev [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , da preprečite okvare prt na teh strojih.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















