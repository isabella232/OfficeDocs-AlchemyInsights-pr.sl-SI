---
title: Ustvarjanje uporabnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: afba00ffc6ba082606e0071b41e2917b11e6a39d61cd0df7e468f0238f2ed8e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118760"
---
# <a name="create-user"></a>Ustvarjanje uporabnika

**OBVESTILO:**

- [Zastaranje podpore za vpis v WebView v Googlu od 4. januarja 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Preverite, ali lahko na vaše aplikacije vplivajo [Googlova navodila](https://go.microsoft.com/fwlink/?linkid=2157323) za preskušanje združljivosti.
- Poskrbite, da boste za vpis uporabnikov s potrošniškimi Google računi uporabljali sistemski spletni pogled ali brskalnik sistema. Če želite več informacij, glejte [Težave pri vpisu v aplikacije le z brskalnikom Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Ne morem ustvariti novega uporabnika v imeniku Azure AD**

1. Prepričajte se, da imate dovoljenje za ustvarjanje novega standardnega uporabnika. Nov standardni uporabnik lahko ustvari le vloga globalnega skrbnika ali Azure Active Directory skrbnika v programu Azure Active Directory (AD). Če niste v eni od teh vlog, prosite skrbnika, da vas doda na eno od teh vlog ali ustvari nov uporabniški račun za vas.
1. Zagotovite, da je uporabniško ime v domeni, ki je potrjena v imeniku Azure AD. Če v imeniku Azure AD ni potrjenih imen domen po meri, lahko uporabite začetno domeno Azure AD, ki se konča z *.onmicrosoft.com.
1. Zagotovite, da je uporabniško ime v domeni, ki ni v domeni Azure AD iz imenika AD na mestu uporabe. Uporabnikov ni mogoče dodati v oblak z imeni domen, ki so povezana z domenami na mestu uporabe.
1. Zagotovite, da noben drug uporabnik ali stik še nima uporabniškega imena, ki ga želite dodeliti novemu uporabniku. Uporabniška imena morajo biti enolična v imeniku Azure AD.
1. Glejte [Vloge in skrbniki imenika Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.
1. Oglejte si [imena domen](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.
1. Preglejte [dnevnike nadzora in](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) si oglejte podrobnejše informacije o nedavno ustvarjenem ali izbrisanem uporabniku, na primer o tem, kdo je izvedel dejanje in kdaj.
1. Če želite več informacij o dodajanju novih uporabnikov, glejte Uporaba portala Azure za [ustvarjanje novega uporabnika v imeniku Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Skrbniške vloge za Azure AD:](/azure/active-directory/active-directory-assign-admin-roles)Skrbniška dovoljenja za vloge v Azure Active Directory
1. Novega uporabnika lahko ustvarite tudi z azure [AD PowerShell.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
