---
title: Težave s poverilnicami
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063688"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="3545b-102">Težave s poverilnicami</span><span class="sxs-lookup"><span data-stu-id="3545b-102">Issues with credentials</span></span>

<span data-ttu-id="3545b-103">[Platforma Microsoft Identity in s tokom poverilnic odjemalca oauth 2,0 je](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) opisano, kako program neposredno v primerjavi s podelitvijo poverilnic odjemalca OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="3545b-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="3545b-104">**Kako upravljam geslo ali poverilnice potrdila programa?**</span><span class="sxs-lookup"><span data-stu-id="3545b-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="3545b-105">V storitvi Azure CLI lahko uporabite [poverilnico programa AZ ad app](https://docs.microsoft.com/cli/azure/ad/app/credential) , če želite izbrisati, zapisati seznam ali ponastaviti geslo za program ali poverilnice potrdila.</span><span class="sxs-lookup"><span data-stu-id="3545b-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="3545b-106">**Kako moji uporabniki ponastavijo gesla?**</span><span class="sxs-lookup"><span data-stu-id="3545b-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="3545b-107">Uporabniki se morajo [registrirati za samopostrežno ponastavitev gesla](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) , preden lahko ponastavijo gesla.</span><span class="sxs-lookup"><span data-stu-id="3545b-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="3545b-108">Ko je uporabnik registriran, lahko v tem članku upoštevajo navodila za ponastavitev gesla: [ponastavitev službenega ali šolskega gesla](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="3545b-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="3545b-109">**Kako moji uporabniki spreminjajo svoja gesla?**</span><span class="sxs-lookup"><span data-stu-id="3545b-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="3545b-110">Uporabniki lahko upoštevajo korake v tem članku, da spremenijo svoja gesla: [Kako spremeniti geslo](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="3545b-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="3545b-111">Prav tako lahko [upravljajo gesla za program za preverjanje v dveh korakih](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="3545b-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="3545b-112">**Moj uporabnik dobi napako pri spreminjanju ali ponastavitvi gesla**</span><span class="sxs-lookup"><span data-stu-id="3545b-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="3545b-113">S to povezavo boste našli informacije o pogostih težavah, ki se lahko pojavijo, ko uporabnik poskuša ponastaviti svoje geslo: [pogoste težave in njihove rešitve](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="3545b-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="3545b-114">**Imam težavo s ponastavitvijo uporabniškega gesla**</span><span class="sxs-lookup"><span data-stu-id="3545b-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="3545b-115">Preverite, ali imate dovoljenje za ponastavitev gesel.</span><span class="sxs-lookup"><span data-stu-id="3545b-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="3545b-116">*Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika.*</span><span class="sxs-lookup"><span data-stu-id="3545b-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3545b-117">Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.</span><span class="sxs-lookup"><span data-stu-id="3545b-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="3545b-118">Prepričajte se, da razumete zahteve za licenciranje:</span><span class="sxs-lookup"><span data-stu-id="3545b-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="3545b-119">Imeti morate vsaj eno licenco, ki je dodeljena v organizaciji:</span><span class="sxs-lookup"><span data-stu-id="3545b-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="3545b-120">**Samo uporabniki v oblaku** – vsak Office 365 (O365) plačan sku ali Azure ad Basic</span><span class="sxs-lookup"><span data-stu-id="3545b-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="3545b-121">**Uporabniki v oblaku in/ali na mestu uporabe** – Azure ad Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure produktivno podjetje (SPE)</span><span class="sxs-lookup"><span data-stu-id="3545b-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="3545b-122">Če želite izvedeti več o zahtevah za licenciranje, glejte [zahteve za licenciranje za samopostrežno ponastavitev gesla za storitev AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="3545b-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="3545b-123">Če želite ponastaviti geslo uporabnika, poiščite uporabnika v storitvi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3545b-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="3545b-124">Nato na rezilu pregled za tega uporabnika kliknite gumb» Ponastavi geslo «.</span><span class="sxs-lookup"><span data-stu-id="3545b-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="3545b-125">**Gumb za ponastavitev gesla je zatemnjen**</span><span class="sxs-lookup"><span data-stu-id="3545b-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="3545b-126">Nimate dovoljenja za ponastavitev gesel **tega** uporabnika.</span><span class="sxs-lookup"><span data-stu-id="3545b-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="3545b-127">*Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika.*</span><span class="sxs-lookup"><span data-stu-id="3545b-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3545b-128">Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.</span><span class="sxs-lookup"><span data-stu-id="3545b-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="3545b-129">**Rezilo za ponastavitev gesla ne vidim**</span><span class="sxs-lookup"><span data-stu-id="3545b-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="3545b-130">Nimate dovoljenja za ponastavitev gesel.</span><span class="sxs-lookup"><span data-stu-id="3545b-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="3545b-131">*Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika.*</span><span class="sxs-lookup"><span data-stu-id="3545b-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3545b-132">Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.</span><span class="sxs-lookup"><span data-stu-id="3545b-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="3545b-133">**V ponastavitev gesla ne vidim rezila za integracijo na mestu uporabe**</span><span class="sxs-lookup"><span data-stu-id="3545b-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="3545b-134">Rezilo integracije na mestu uporabe je prikazano le v hibridnih okoljih, kar pomeni, da uporabljate geslo nepotrjenim za manipuliranje uporabnikovih gesel na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="3545b-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="3545b-135">Tega rezila ne vidite, če:</span><span class="sxs-lookup"><span data-stu-id="3545b-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="3545b-136">Ne uporabljate gesla nepotrjenim</span><span class="sxs-lookup"><span data-stu-id="3545b-136">You are not using password writeback</span></span>
  - <span data-ttu-id="3545b-137">Prišlo je do težave z namestitvijo/povezljivostjo gesla nepotrjenim</span><span class="sxs-lookup"><span data-stu-id="3545b-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="3545b-138">Prišlo je do težave z namestitvijo/povezljivostjo storitve Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="3545b-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="3545b-139">Če želite več korakov za odpravljanje težav z geslom nepotrjenim, glejte [Odpravljanje težav z geslom nepotrjenim](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="3545b-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="3545b-140">**Ne vem, kako ponastavim geslo uporabnika**</span><span class="sxs-lookup"><span data-stu-id="3545b-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="3545b-141">Vpišite se v portal Azure kot ustrezen skrbnik.</span><span class="sxs-lookup"><span data-stu-id="3545b-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="3545b-142">Pojdite na rezilo **uporabnikov in skupin** , izberite **vsi uporabniki**.</span><span class="sxs-lookup"><span data-stu-id="3545b-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="3545b-143">Izberite uporabnika s seznama.</span><span class="sxs-lookup"><span data-stu-id="3545b-143">Select a user from the list.</span></span>
4. <span data-ttu-id="3545b-144">Za izbranega uporabnika izberite **pregled** in nato v ukazni vrstici izberite **Ponastavi geslo**.</span><span class="sxs-lookup"><span data-stu-id="3545b-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="3545b-145">Izberite gumb za **ponastavitev gesla** in sledite navodilom na zaslonu.</span><span class="sxs-lookup"><span data-stu-id="3545b-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="3545b-146">Le ponastavi, izvedeno prek nepotrjenim gesla za podporo **portala Azure** .</span><span class="sxs-lookup"><span data-stu-id="3545b-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="3545b-147">**Z geslom uporabnika na mestu uporabe v skrbniškem portalu za Office 365 ali v mobilnem programu Office 365 se uporabnik še vedno ne more vpisati**</span><span class="sxs-lookup"><span data-stu-id="3545b-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="3545b-148">V tem portalu ni podprt Nepotrjenim za gesla.</span><span class="sxs-lookup"><span data-stu-id="3545b-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="3545b-149">Znova ponastavite geslo uporabnika v portalu Azure.</span><span class="sxs-lookup"><span data-stu-id="3545b-149">Reset the user's password again in the Azure portal.</span></span>
