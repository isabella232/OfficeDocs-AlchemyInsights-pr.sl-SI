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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747027"
---
# <a name="create-user"></a>Ustvarjanje uporabnika

**Napoved**

- Zastaranje [podpore za vpis v storitev Google z začetkom januar 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Preverite, ali bodo vaše aplikacije morda vplivale na [navodila za Google](https://go.microsoft.com/fwlink/?linkid=2157323) za preskušanje združljivosti.
- Če se želite prijaviti v uporabnike s storitvijo Google računi za potrošnike, se prepričajte, da uporabljate sistemski spletni pogled ali sistem brskalnika. Če želite več informacij, glejte [težave pri vpisu v program le z brskalnikom Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Ne morem ustvariti novega uporabnika v imeniku Azure AD Directory**

1. Zagotovite, da imate dovoljenje za ustvarjanje novega standardnega uporabnika. V storitvi Azure Active Directory (AD) lahko ustvari novega standardnega uporabnika le globalni skrbnik ali skrbnik uporabnika. Če niste v eni od teh vlog, prosite skrbnika, da vas doda v eno od teh vlog, ali pa ustvarite nov uporabniški račun.
1. Zagotovite, da je uporabniško ime v domeni, ki je preverjena v storitvi Azure AD. Če nimate preverjenih imen domen po meri v storitvi Azure AD, lahko uporabite začetno domeno storitve Azure AD, ki se konča z *. onmicrosoft.com.
1. Zagotovite, da je uporabniško ime v domeni, ki ni Združeno do storitve Azure AD iz OGLASa na mestu uporabe. Uporabnikov ni mogoče dodati v oblak z imeni domen, ki so Združene od na mestu uporabe.
1. Zagotovite, da noben drug uporabnik ali stik že nima uporabniško ime, ki ga želite dodeliti novemu uporabniku. Uporabniška imena morajo biti enolična v storitvi Azure AD.
1. Glejte [vloge za AZURE ad in skrbnike](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za vaš oglas Azure.
1. Glejte [imena domen](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za svoj oglas Azure.
1. Preglejte [dnevnike nadzora](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) , če si želite ogledati podrobnejše informacije o nedavno ustvarjenem ali izbrisanem uporabniku, kot je bil izveden postopek in kdaj.
1. Če želite več informacij o dodajanju novih uporabnikov, [si oglejte Uporaba portala Azure za ustvarjanje novega uporabnika v storitvi AZURE ad](/azure/active-directory/active-directory-users-create-azure-portal).
1. [Skrbniške vloge za AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): dovoljenja skrbniških vlog v imeniku Azure Active Directory
1. [Če želite ustvariti novega uporabnika, lahko uporabite tudi AZURE ad PowerShell](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
