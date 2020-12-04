---
title: Odpravljanje težav s storitvijo PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573901"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="4d7f4-102">Odpravljanje težav s storitvijo PRT</span><span class="sxs-lookup"><span data-stu-id="4d7f4-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="4d7f4-103">Za katero koli napravo, ki bo dokončana s preverjeno pristnostjo, mora biti v celoti registrirana in v dobrem stanju ter sposobna pridobiti primarni žeton za osveževanje (PRT).</span><span class="sxs-lookup"><span data-stu-id="4d7f4-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="4d7f4-104">Postopek registracije hibridne Azure AD JOIN zahteva, da so naprave v omrežju podjetja.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="4d7f4-105">Deluje tudi prek omrežja VPN, vendar je na tem mestu nekaj opozoril.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="4d7f4-106">Slišali smo, da stranke potrebujejo pomoč pri odpravljanju težav s procesom registracije hibridne Azure AD, ki je v skladu s pogoji oddaljenega dela.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="4d7f4-107">Tukaj je razčlenitev, kaj se dogaja pod kapuco med postopkom registracije.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="4d7f4-108">**Okolje za preverjanje pristnosti v oblaku (s sinhronizacijo sinhronizacije z geslom Azure AD ali prepustnim preverjanjem)**</span><span class="sxs-lookup"><span data-stu-id="4d7f4-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="4d7f4-109">Ta potek registracije je poznan tudi kot» sinhronizacija JOIN «.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="4d7f4-110">Windows 10 odkrije zapis SCP, ko se uporabnik prijavi v napravo.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="4d7f4-111">Naprava najprej poskuša pridobiti podatke najemnika na strani odjemalca SCP v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="4d7f4-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="4d7f4-112">Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="4d7f4-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="4d7f4-113">Če ne uspe, naprava komunicira z imenikom Active Directory na mestu uporabe (AD), da pridobi informacije o najemniku iz stične povezave storitve (SCP).</span><span class="sxs-lookup"><span data-stu-id="4d7f4-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="4d7f4-114">Če želite preveriti SCP, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="4d7f4-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="4d7f4-115">Priporočamo, da omogočite SCP v OGLASu in uporabljate le odjemalca SCP za začetno preverjanje veljavnosti.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="4d7f4-116">Windows 10 poskuša komunicirati s storitvijo Azure AD v okviru sistemskega konteksta, da se preveri pristnost pred storitvijo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="4d7f4-117">Preverite lahko, ali ima naprava dostop do Microsoftovih virov v okviru sistemskega računa, in sicer tako, da uporabi skriptno povezljivost za preskusno napravo.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="4d7f4-118">Windows 10 ustvari samopodpisano potrdilo in ga shrani pod računalnikov predmet v OGLASu na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="4d7f4-119">Za to morate uporabiti krmilnik domene.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="4d7f4-120">Predmet naprave, ki ima potrdilo, je sinhroniziran s storitvijo Azure AD s povezavo» Azure AD Connect «.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="4d7f4-121">Cikel sinhronizacije je privzeto vsakih 30 minut, vendar je odvisen od konfiguracije povezave s storitvijo Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="4d7f4-122">Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="4d7f4-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="4d7f4-123">Na tej stopnji lahko vidite napravo» zadeva «v razdelku» čakajoče «v razdelku» rezilo «portala Azure.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="4d7f4-124">Pri naslednjem vpisu uporabnika v sistem Windows 10 bo registracija dokončana.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="4d7f4-125">Če uporabljate VPN in je postopek prijave odjave končan, lahko ročno sprožite registracijo:</span><span class="sxs-lookup"><span data-stu-id="4d7f4-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="4d7f4-126">Izdaja dsregcmd/JOIN lokalno v skrbniškem pozivniku ali oddaljeno prek PSExec v računalnik s sistemom Windows.</span><span class="sxs-lookup"><span data-stu-id="4d7f4-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="4d7f4-127">Na primer PsExec-s \\ win10client01 cmd, dsregcmd/JOIN</span><span class="sxs-lookup"><span data-stu-id="4d7f4-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="4d7f4-128">Če želite več podrobnosti o hibridnih težavah z združevanjem, glejte [Odpravljanje težav z napravami](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="4d7f4-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
