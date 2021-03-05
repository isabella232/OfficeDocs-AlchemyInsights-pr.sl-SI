---
title: Sinhronizacija gesel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483084"
---
# <a name="password-synchronization"></a><span data-ttu-id="6c82f-102">Sinhronizacija gesel</span><span class="sxs-lookup"><span data-stu-id="6c82f-102">Password synchronization</span></span>

<span data-ttu-id="6c82f-103">**Sinhronizacija gesel za gesla sploh ne deluje**</span><span class="sxs-lookup"><span data-stu-id="6c82f-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="6c82f-104">Nekatere pogoste težave, s katerimi se srečujejo uporabniki, ko sinhronizacija z geslom ne deluje:</span><span class="sxs-lookup"><span data-stu-id="6c82f-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="6c82f-105">Račun imenika Active Directory, ki ga uporablja storitev Azure AD Connect za komunikacijo z imenikom Active Directory na mestu uporabe, ni dodeljen za **ponovitev imenika** in **ponovitev imenika spremeni vsa** dovoljenja, ki jih potrebujete za sinhronizacijo gesel – to morate popraviti tako, da dodelite ta dovoljenja v račun imenika Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6c82f-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="6c82f-106">Sinhronizacija z geslom za razprševanje je onemogočena, ko je skrbnik **spremenil funkcijo uporabnika** Sign-In iz **sinhronizacije z geslom** na drugo možnost, kot je na primer **zveza z AD FS** v čarovniku za povezovanje v storitvi Azure ad Connect.</span><span class="sxs-lookup"><span data-stu-id="6c82f-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="6c82f-107">Težave s povezljivostjo z imenikom Active Directory na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="6c82f-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="6c82f-108">Na primer nekateri krmilniki domen niso dostopni za povezavo s storitvijo Azure AD Connect ali pa so [vrata](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) blokirana s požarnim zidom – to morate popraviti tako, da zagotovite, da je povezljivost med povezovanjem s STREŽNIKOM Azure ad Connect Server in imenikom Active Directory pravilno delovala.</span><span class="sxs-lookup"><span data-stu-id="6c82f-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="6c82f-109">Strežnik Azure AD Connect Server trenutno poteka v načinu uprizoritev, zaradi česar se strežnik ne more razpršiti z geslom – če želite odpraviti težavo, upoštevajte navodila, opisana v razdelku [Odpravljanje težav z sinhronizacijo gesel s sinhronizacijo storitve AZURE ad Connect – nobena gesla niso sinhronizirana](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="6c82f-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="6c82f-110">**Sinhronizacija gesel za gesla ne deluje za nekatere uporabnike**</span><span class="sxs-lookup"><span data-stu-id="6c82f-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="6c82f-111">Če ste opazili, da HASH gesla ni sinhroniziran za uporabnika, uporabite opravilo za **Odpravljanje težav** v storitvi Azure ad Connect, da razišče in odpravite težavo.</span><span class="sxs-lookup"><span data-stu-id="6c82f-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="6c82f-112">Izvedite ta opravila:</span><span class="sxs-lookup"><span data-stu-id="6c82f-112">Perform the following tasks:</span></span>

    <span data-ttu-id="6c82f-113">v.</span><span class="sxs-lookup"><span data-stu-id="6c82f-113">a.</span></span> [<span data-ttu-id="6c82f-114">Zagon opravila za odpravljanje težav v čarovniku</span><span class="sxs-lookup"><span data-stu-id="6c82f-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="6c82f-115">b.</span><span class="sxs-lookup"><span data-stu-id="6c82f-115">b.</span></span> [<span data-ttu-id="6c82f-116">Uporaba ukaza» cmdlet «za odpravljanje težav pri preverjanju težave pri sinhronizaciji gesel za določeno uporabo</span><span class="sxs-lookup"><span data-stu-id="6c82f-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="6c82f-117">Uporabniški predmet uporabnika na mestu uporabe je omogočen za **uporabnika mora spremeniti geslo ob naslednji možnosti prijave** .</span><span class="sxs-lookup"><span data-stu-id="6c82f-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="6c82f-118">Ko je ta možnost omogočena, je uporabniku dodeljeno začasno geslo in pozvani boste, da spremenite geslo v naslednji prijavi.</span><span class="sxs-lookup"><span data-stu-id="6c82f-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="6c82f-119">Azure AD Connect ne sinhronizira začasnih gesel s storitvijo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c82f-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="6c82f-120">Če želite odpraviti zgoraj navedeno težavo, izvedite eno od teh opravil:</span><span class="sxs-lookup"><span data-stu-id="6c82f-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="6c82f-121">Prosite uporabnika, naj se vpiše v program na mestu uporabe (na primer namizje sistema Windows), in spremenite geslo.</span><span class="sxs-lookup"><span data-stu-id="6c82f-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="6c82f-122">Novo geslo bo sinhronizirano s storitvijo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c82f-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="6c82f-123">Naj skrbnik posodobi uporabnikovo geslo, ne da bi omogočil, da **mora uporabnik spremeniti geslo ob naslednji prijavi** in dati v skupno rabo novo geslo za uporabnika.</span><span class="sxs-lookup"><span data-stu-id="6c82f-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="6c82f-124">Predmet uporabnika imenika Active Directory na mestu uporabe ni **pravilno konfiguriran** za sinhronizacijo predmetov ali sinhronizacijo gesla.</span><span class="sxs-lookup"><span data-stu-id="6c82f-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="6c82f-125">Če želite odpraviti to težavo, upoštevajte navodila, opisana v razdelku [Odpravljanje težav z razprševanjem gesel s sinhronizacijo storitve AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="6c82f-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







