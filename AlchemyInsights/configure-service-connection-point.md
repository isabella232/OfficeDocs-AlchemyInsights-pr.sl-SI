---
title: Konfiguracija točkovne povezave storitve (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037289"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="a1e07-102">Konfiguracija točkovne povezave storitve (SCP)</span><span class="sxs-lookup"><span data-stu-id="a1e07-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="a1e07-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="a1e07-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="a1e07-104">**Razlog**: ne morem prebrati predmeta SCP in pridobiti informacije o najemniku v storitvi Azure ad</span><span class="sxs-lookup"><span data-stu-id="a1e07-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="a1e07-105">**Resolucija**: glejte razdelek [Konfiguracija točke povezave storitve](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="a1e07-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="a1e07-106">**Akcijski načrt**</span><span class="sxs-lookup"><span data-stu-id="a1e07-106">**Action plan**</span></span>

- <span data-ttu-id="a1e07-107">Preverite, ali je naprava prejela GPO za nadzorovano preverjanje veljavnosti.</span><span class="sxs-lookup"><span data-stu-id="a1e07-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="a1e07-108">Zagotovite, da je GPO ustvaril registrske ključe.</span><span class="sxs-lookup"><span data-stu-id="a1e07-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="a1e07-109">Zagotovite, da imate 2 tipki, ustvarjeni z ID-jem imenika in domeno onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="a1e07-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="a1e07-110">**Konfiguracija nastavitve registra odjemalca za SCP**</span><span class="sxs-lookup"><span data-stu-id="a1e07-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="a1e07-111">Uporabite ta primer, če želite ustvariti predmet pravilnika skupine (GPO), da uvedete nastavitev registra, ki konfigurira vnos SCP v registru naprav.</span><span class="sxs-lookup"><span data-stu-id="a1e07-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="a1e07-112">Odprite konzolo za upravljanje pravilnika skupine in ustvarite nov GPO v svoji domeni.</span><span class="sxs-lookup"><span data-stu-id="a1e07-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="a1e07-113">Navedite novo ustvarjeno GPO ime (na primer ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="a1e07-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="a1e07-114">Uredite GPO in poiščite to pot: **Konfiguracija računalnika > nastavitve > nastavitve sistema Windows > register**.</span><span class="sxs-lookup"><span data-stu-id="a1e07-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="a1e07-115">Z desno tipko miške kliknite **register** in izberite **nov > element registra**.</span><span class="sxs-lookup"><span data-stu-id="a1e07-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="a1e07-116">Na zavihku **splošno** konfigurirajte to:</span><span class="sxs-lookup"><span data-stu-id="a1e07-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="a1e07-117">**Dejanje**: posodobitev</span><span class="sxs-lookup"><span data-stu-id="a1e07-117">**Action**: Update</span></span>
    
- <span data-ttu-id="a1e07-118">**Panj**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="a1e07-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="a1e07-119">**Pot ključa**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="a1e07-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="a1e07-120">**Ime vrednosti**: TenantId</span><span class="sxs-lookup"><span data-stu-id="a1e07-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="a1e07-121">**Vrsta vrednosti**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="a1e07-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="a1e07-122">**Podatki o vrednosti**: GUID ali ID imenika vašega primerka za Azure ad (to vrednost je mogoče najti v **portalu Azure > azure Active Directory > lastnosti > Directory ID**)</span><span class="sxs-lookup"><span data-stu-id="a1e07-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="a1e07-123">Kliknite **V redu**.</span><span class="sxs-lookup"><span data-stu-id="a1e07-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="a1e07-124">Z desno tipko miške kliknite **register** in izberite **nov > element registra**.</span><span class="sxs-lookup"><span data-stu-id="a1e07-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="a1e07-125">Na zavihku **splošno** konfigurirajte to:</span><span class="sxs-lookup"><span data-stu-id="a1e07-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="a1e07-126">**Dejanje**: posodobitev</span><span class="sxs-lookup"><span data-stu-id="a1e07-126">**Action**: Update</span></span>
    
- <span data-ttu-id="a1e07-127">**Panj**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="a1e07-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="a1e07-128">**Pot ključa**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="a1e07-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="a1e07-129">**Ime vrednosti**: TenantName</span><span class="sxs-lookup"><span data-stu-id="a1e07-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="a1e07-130">**Vrsta vrednosti**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="a1e07-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="a1e07-131">**Podatki o vrednosti**: preverjeno ime domene, če uporabljate Združeno okolje, kot je AD FS.</span><span class="sxs-lookup"><span data-stu-id="a1e07-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="a1e07-132">Ime preverjene domene ali ime domene onmicrosoft.com (na primer contoso. onmicrosoft). com, če uporabljate upravljano okolje</span><span class="sxs-lookup"><span data-stu-id="a1e07-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="a1e07-133">Kliknite **V redu**.</span><span class="sxs-lookup"><span data-stu-id="a1e07-133">Click **OK**.</span></span>

7. <span data-ttu-id="a1e07-134">Zaprite urejevalnik za novo ustvarjeni GPO.</span><span class="sxs-lookup"><span data-stu-id="a1e07-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="a1e07-135">Povežite novo ustvarjeni GPO na želeno mesto, ki vsebuje računalnike, ki so povezani z domeno, ki pripadajo vaši nadzorovani populaciji za širitev.</span><span class="sxs-lookup"><span data-stu-id="a1e07-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="a1e07-136">Če želite več informacij, glejte [nadzorovana Validacija hibridnega združevanja v storitvi AZURE ad – AZURE ad | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) in  [Odpravljanje težav z naprednimi napravami v hibridni storitvi Azure Active Directory | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="a1e07-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









