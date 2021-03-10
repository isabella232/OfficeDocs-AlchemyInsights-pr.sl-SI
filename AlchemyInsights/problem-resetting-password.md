---
title: Težava pri ponastavitvi gesla
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696278"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="2cd03-102">Težave s ponastavitvijo gesla</span><span class="sxs-lookup"><span data-stu-id="2cd03-102">Problems resetting password</span></span>

<span data-ttu-id="2cd03-103">Spodaj je navedenih nekaj težav, s katerimi se lahko soočite pri ponastavitvi gesla in možnih rešitvah:</span><span class="sxs-lookup"><span data-stu-id="2cd03-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="2cd03-104">**Imam težavo z ponastavitev gesla, ki ni zajeta v drugih kategorijah**</span><span class="sxs-lookup"><span data-stu-id="2cd03-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="2cd03-105">Zagotovite, da imate dovoljenje za ponastavitev gesel.</span><span class="sxs-lookup"><span data-stu-id="2cd03-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="2cd03-106">Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika.</span><span class="sxs-lookup"><span data-stu-id="2cd03-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="2cd03-107">Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.</span><span class="sxs-lookup"><span data-stu-id="2cd03-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="2cd03-108">Zagotovite, da razumete zahteve za licenciranje:</span><span class="sxs-lookup"><span data-stu-id="2cd03-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="2cd03-109">Imeti morate vsaj eno licenco, dodeljeno v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="2cd03-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="2cd03-110">Samo uporabniki v oblaku – vsak Office 365 (O365) plačan SKU ali Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="2cd03-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="2cd03-111">Uporabniki v oblaku in/ali na mestu uporabe – Azure AD Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure produktivno podjetje (SPE)</span><span class="sxs-lookup"><span data-stu-id="2cd03-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="2cd03-112">Če želite več informacij o zahtevah za licenciranje, si oglejte članek [zahteve za licenciranje za samopostrežno ponastavitev gesla za AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="2cd03-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="2cd03-113">**Imam težave pri testiranju pravilnika za ponastavitev gesla, ki sem ga nastavil**</span><span class="sxs-lookup"><span data-stu-id="2cd03-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="2cd03-114">Nedavno uporabljene pravilnike lahko traja nekaj minut, da se replicirajo v vseh podatkovnih centrih in končnih točkah.</span><span class="sxs-lookup"><span data-stu-id="2cd03-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="2cd03-115">Fizična razdalja od podatkovnega središča bo vplivala tudi na to, kako hitro se spremembe izvajajo.</span><span class="sxs-lookup"><span data-stu-id="2cd03-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="2cd03-116">Preskusite s končnim uporabnikom, ne skrbnikom, in pilot z majhnim naborom uporabnikov.</span><span class="sxs-lookup"><span data-stu-id="2cd03-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="2cd03-117">Pravilniki, konfigurirani v portalu Azure, veljajo le za končne uporabnike, ne skrbnike.</span><span class="sxs-lookup"><span data-stu-id="2cd03-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="2cd03-118">Microsoft uveljavi močne privzete pravilnike za ponastavitev gesla za vse funkcije za skrbnike v storitvi Azure (primer: globalni skrbnik, skrbnik za pomoč, skrbnik za gesla itd.)</span><span class="sxs-lookup"><span data-stu-id="2cd03-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="2cd03-119">Preberite več o [pravilnikih za skrbnike](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="2cd03-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="2cd03-120">**Želim uvesti ponastavitev gesla, vendar ne želim, da moji uporabniki registrirajo dodatne varnostne informacije**</span><span class="sxs-lookup"><span data-stu-id="2cd03-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="2cd03-121">Vnaprej zapolnijo podatke za svoje uporabnike, tako da jim ni treba!</span><span class="sxs-lookup"><span data-stu-id="2cd03-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="2cd03-122">-Kot skrbnik lahko nastavite lastnosti telefona in e-pošte za uporabnike pred uvajanjem ponastavitev gesla v vašo organizacijo.</span><span class="sxs-lookup"><span data-stu-id="2cd03-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="2cd03-123">To lahko naredite z uporabo vmesnika API, PowerShell ali Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="2cd03-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="2cd03-124">Več informacij najdete tukaj:</span><span class="sxs-lookup"><span data-stu-id="2cd03-124">More information here:</span></span>
- [<span data-ttu-id="2cd03-125">Uvajanje ponastavitev gesla brez zahteve za registracijo uporabnikov</span><span class="sxs-lookup"><span data-stu-id="2cd03-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="2cd03-126">Katere podatke uporablja ponastavitev gesla</span><span class="sxs-lookup"><span data-stu-id="2cd03-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="2cd03-127">**Gumb za ponastavitev gesla je zatemnjen**</span><span class="sxs-lookup"><span data-stu-id="2cd03-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="2cd03-128">Nimate dovoljenja za ponastavitev gesel tega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="2cd03-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="2cd03-129">Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika.</span><span class="sxs-lookup"><span data-stu-id="2cd03-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="2cd03-130">Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.</span><span class="sxs-lookup"><span data-stu-id="2cd03-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="2cd03-131">**Rezilo za ponastavitev gesla ne vidim**</span><span class="sxs-lookup"><span data-stu-id="2cd03-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="2cd03-132">Nimate dovoljenja za ponastavitev gesel.</span><span class="sxs-lookup"><span data-stu-id="2cd03-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="2cd03-133">Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika.</span><span class="sxs-lookup"><span data-stu-id="2cd03-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="2cd03-134">Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.</span><span class="sxs-lookup"><span data-stu-id="2cd03-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="2cd03-135">**V ponastavitev gesla ne vidim rezila za integracijo na mestu uporabe**</span><span class="sxs-lookup"><span data-stu-id="2cd03-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="2cd03-136">Rezilo integracije na mestu uporabe je prikazano le v hibridnih okoljih, kar pomeni, da uporabljate geslo nepotrjenim za manipuliranje uporabnikovih gesel na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="2cd03-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="2cd03-137">Tega rezila ne vidite, če:</span><span class="sxs-lookup"><span data-stu-id="2cd03-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="2cd03-138">Ne uporabljate gesla nepotrjenim</span><span class="sxs-lookup"><span data-stu-id="2cd03-138">You are not using password writeback</span></span>
    - <span data-ttu-id="2cd03-139">Prišlo je do težave z namestitvijo/povezljivostjo gesla nepotrjenim</span><span class="sxs-lookup"><span data-stu-id="2cd03-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="2cd03-140">Prišlo je do težave z namestitvijo/povezljivostjo storitve Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="2cd03-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="2cd03-141">Če želite več korakov za odpravljanje težav z geslom nepotrjenim, glejte razdelek [Odpravljanje težav z geslom nepotrjenim](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="2cd03-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="2cd03-142">**Ne vem, kako ponastavim geslo uporabnika**</span><span class="sxs-lookup"><span data-stu-id="2cd03-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="2cd03-143">Vpišite se v portal Azure kot ustrezen skrbnik.</span><span class="sxs-lookup"><span data-stu-id="2cd03-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="2cd03-144">Pojdite na rezilo uporabnikov in skupin, izberite **vsi uporabniki**.</span><span class="sxs-lookup"><span data-stu-id="2cd03-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="2cd03-145">Izberite uporabnika s seznama.</span><span class="sxs-lookup"><span data-stu-id="2cd03-145">Select a user from the list.</span></span>
1. <span data-ttu-id="2cd03-146">Za izbranega uporabnika izberite **pregled** in nato v ukazni vrstici kliknite **Ponastavi geslo**.</span><span class="sxs-lookup"><span data-stu-id="2cd03-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="2cd03-147">Sledite navodilom na zaslonu.</span><span class="sxs-lookup"><span data-stu-id="2cd03-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="2cd03-148">Le ponastavi, izvedeno prek nepotrjenim gesla za podporo portala Azure.</span><span class="sxs-lookup"><span data-stu-id="2cd03-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="2cd03-149">**Z geslom uporabnika na mestu uporabe v skrbniškem portalu za Office 365 ali v mobilnem programu Office 365 se uporabnik še vedno ne more vpisati**</span><span class="sxs-lookup"><span data-stu-id="2cd03-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="2cd03-150">V tem portalu ni podprt Nepotrjenim za gesla.</span><span class="sxs-lookup"><span data-stu-id="2cd03-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="2cd03-151">Znova ponastavite geslo uporabnika v portalu Azure – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="2cd03-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

