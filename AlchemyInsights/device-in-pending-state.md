---
title: Naprava v čakajočem stanju
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679992"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="307f8-102">Naprava v čakajočem stanju</span><span class="sxs-lookup"><span data-stu-id="307f8-102">Device in pending state</span></span>

<span data-ttu-id="307f8-103">**Predpogoji**</span><span class="sxs-lookup"><span data-stu-id="307f8-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="307f8-104">Če prvič nastavljate registracije naprav, zagotovite, da ste pregledali [Uvod v upravljanje naprav v storitvi Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , ki vas bo vodil o tem, kako pridobite naprave pod nadzorom storitve Azure ad.</span><span class="sxs-lookup"><span data-stu-id="307f8-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="307f8-105">Če želite neposredno registrirati naprave v storitvi Azure AD in jih vpisati v InTune, boste morali zagotoviti, da ste [konfigurirali InTune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) in imate na prvem mestu [licence](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .</span><span class="sxs-lookup"><span data-stu-id="307f8-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="307f8-106">Zagotovite, da imate dovoljenje za izvajanje operacij v storitvi Azure AD in AD na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="307f8-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="307f8-107">Nastavitve za registracije naprave lahko upravljajo le globalni skrbnik v storitvi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="307f8-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="307f8-108">Če želite nastaviti samodejne registracije v imeniku Active Directory na mestu uporabe, morate biti skrbnik imenika Active Directory in AD FS (po potrebi).</span><span class="sxs-lookup"><span data-stu-id="307f8-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="307f8-109">Postopek registracije hibridne Azure AD JOIN zahteva, da so naprave v omrežju podjetja.</span><span class="sxs-lookup"><span data-stu-id="307f8-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="307f8-110">Deluje tudi prek omrežja VPN, vendar je na tem mestu nekaj opozoril.</span><span class="sxs-lookup"><span data-stu-id="307f8-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="307f8-111">Slišali smo, da stranke potrebujejo pomoč pri odpravljanju težav s procesom registracije hibridne Azure AD v razdelku oddaljene delovne okoliščine.</span><span class="sxs-lookup"><span data-stu-id="307f8-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="307f8-112">**Okolje za preverjanje pristnosti v oblaku (s sinhronizacijo sinhronizacije z geslom Azure AD ali prepustnim preverjanjem)**</span><span class="sxs-lookup"><span data-stu-id="307f8-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="307f8-113">Ta potek registracije je poznan tudi kot» sinhronizacija JOIN «.</span><span class="sxs-lookup"><span data-stu-id="307f8-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="307f8-114">Tukaj je razdelitev tega, kaj se zgodi med postopkom registracije:</span><span class="sxs-lookup"><span data-stu-id="307f8-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="307f8-115">Windows 10 odkrije (SCP), ko se uporabnik prijavi v napravo.</span><span class="sxs-lookup"><span data-stu-id="307f8-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="307f8-116">Naprava najprej poskuša pridobiti podatke najemnika na strani odjemalca SCP v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="307f8-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="307f8-117">Če želite več informacij, glejte [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="307f8-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="307f8-118">Če ne uspe, naprava komunicira z imenikom Active Directory na mestu uporabe, da pridobi informacije o najemniku iz SCP.</span><span class="sxs-lookup"><span data-stu-id="307f8-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="307f8-119">Če želite preveriti SCP, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="307f8-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="307f8-120">Priporočamo, da omogočite SCP v imeniku Active Directory in uporabljate le odjemalca SCP za začetno preverjanje veljavnosti.</span><span class="sxs-lookup"><span data-stu-id="307f8-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="307f8-121">Windows 10 poskuša komunicirati s storitvijo Azure AD v okviru sistemskega konteksta, da se preveri pristnost pred storitvijo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="307f8-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="307f8-122">Preverite lahko, ali ima naprava dostop do Microsoftovih virov v okviru sistemskega računa, in sicer tako, da uporabi [skriptno povezljivost za preskusno napravo](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="307f8-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="307f8-123">Windows 10 ustvari samopodpisano potrdilo in ga shrani pod računalnikov predmet v imeniku Active Directory na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="307f8-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="307f8-124">Za to morate uporabiti krmilnik domene.</span><span class="sxs-lookup"><span data-stu-id="307f8-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="307f8-125">Predmet naprave, ki ima potrdilo, je sinhroniziran s storitvijo Azure AD s povezavo» Azure AD Connect «.</span><span class="sxs-lookup"><span data-stu-id="307f8-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="307f8-126">Cikel sinhronizacije je privzeto vsakih 30 minut, vendar je odvisen od konfiguracije povezave s storitvijo Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="307f8-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="307f8-127">Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="307f8-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="307f8-128">Na tej stopnji lahko vidite napravo» zadeva «v razdelku»**čakajoče**«v razdelku» rezilo «portala Azure.</span><span class="sxs-lookup"><span data-stu-id="307f8-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="307f8-129">Pri naslednjem vpisu uporabnika v sistem Windows 10 bo registracija dokončana.</span><span class="sxs-lookup"><span data-stu-id="307f8-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="307f8-130">Če uporabljate VPN in odjavo/prijava prekine povezljivost domene, lahko ročno sprožite registracijo.</span><span class="sxs-lookup"><span data-stu-id="307f8-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="307f8-131">To naredite tako:</span><span class="sxs-lookup"><span data-stu-id="307f8-131">To do that:</span></span>
    >
    > <span data-ttu-id="307f8-132">Izdaja `dsregcmd /join` lokalno v skrbniškem pozivniku ali oddaljeno prek PSExec v računalnik s sistemom Windows.</span><span class="sxs-lookup"><span data-stu-id="307f8-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="307f8-133">Na primer: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="307f8-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="307f8-134">Če želite pogoste težave z registracijo naprave Azure Active Directory, glejte [pogosta vprašanja o napravah](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="307f8-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
