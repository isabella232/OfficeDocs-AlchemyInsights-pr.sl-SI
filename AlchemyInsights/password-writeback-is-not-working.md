---
title: Geslo Nepotrjenim ne deluje
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243523"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="4fe9b-102">Geslo Nepotrjenim ne deluje</span><span class="sxs-lookup"><span data-stu-id="4fe9b-102">Password Writeback is not working</span></span>

<span data-ttu-id="4fe9b-103">**Imam težave pri konfiguraciji gesla nepotrjenim**</span><span class="sxs-lookup"><span data-stu-id="4fe9b-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="4fe9b-104">Geslo nepotrjenim je funkcija Premium.</span><span class="sxs-lookup"><span data-stu-id="4fe9b-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="4fe9b-105">Prepričajte se, da razumete zahteve za licenciranje:</span><span class="sxs-lookup"><span data-stu-id="4fe9b-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="4fe9b-106">Imeti morate vsaj eno licenco, dodeljeno v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="4fe9b-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="4fe9b-107">**Samo uporabniki v oblaku** – vsak Office 365 (O365) plačan sku ali Azure ad Basic</span><span class="sxs-lookup"><span data-stu-id="4fe9b-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="4fe9b-108">**Uporabniki v oblaku in/ali na mestu uporabe** – Azure ad Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure produktivno podjetje (SPE)</span><span class="sxs-lookup"><span data-stu-id="4fe9b-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="4fe9b-109">Če želite izvedeti več o zahtevah za licenciranje, glejte [zahteve za licenciranje za samopostrežno ponastavitev gesla za AZURE ad.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="4fe9b-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="4fe9b-110">Imate vsaj en skrbniški račun in en preskusni uporabniški račun z eno od ustreznih licenc.</span><span class="sxs-lookup"><span data-stu-id="4fe9b-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="4fe9b-111">Če želite delati z geslom za nepotrjenim, morate povezati Azure AD, da se povežete z Emulatorjem primarnega krmilnika domene.</span><span class="sxs-lookup"><span data-stu-id="4fe9b-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="4fe9b-112">Če želite uporabiti primarni krmilnik domene, lahko konfigurirate povezavo storitve Azure AD, tako da z desno tipko miške kliknete **lastnosti** povezovalnika imenika Active Directory in nato izberete **Konfiguracija particij imenikov**.</span><span class="sxs-lookup"><span data-stu-id="4fe9b-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="4fe9b-113">V razdelku poiščite razdelek **Nastavitve povezave krmilnika domene** in potrdite polje z naslovom **uporabi le želene krmilnike domene**.</span><span class="sxs-lookup"><span data-stu-id="4fe9b-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="4fe9b-114">Če želeni DC ni Emulator PDC, bo Azure AD Connect še vedno vzpostavil dostop do PDC za geslo nepotrjenim.</span><span class="sxs-lookup"><span data-stu-id="4fe9b-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="4fe9b-115">Ponastavitev gesla je bilo konfigurirano in omogočeno v najemniku.</span><span class="sxs-lookup"><span data-stu-id="4fe9b-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="4fe9b-116">Če želite več informacij, glejte [Omogočanje uporabnikom, da ponastavijo gesla za AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="4fe9b-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="4fe9b-117">Prepričajte se, da je skrbniški račun uporabljen za omogočanje gesla Nepotrjenim je skrbniški račun za oblak (ustvarjen v storitvi Azure AD not AD na mestu uporabe)</span><span class="sxs-lookup"><span data-stu-id="4fe9b-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="4fe9b-118">Imate eno ali več-gozdno uvajanje na mestu uporabe s sistemom Windows Server 2008 R2, Windows Server 2012 ali Windows Server 2012 R2 z nameščenimi najnovejšimi servisnimi paketi</span><span class="sxs-lookup"><span data-stu-id="4fe9b-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="4fe9b-119">Imate nameščeno orodje za povezovanje v storitvi Azure AD in ste pripravili svoje OGLAŠEVALsko okolje za sinhronizacijo z oblakom.</span><span class="sxs-lookup"><span data-stu-id="4fe9b-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="4fe9b-120">Preden preskusite geslo za nepotrjenim, se prepričajte, da ste najprej dokončali popolno uvoz in popolno sinhronizacijo iz oglasov AD in Azure AD v storitvi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="4fe9b-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="4fe9b-121">Če želite izvedeti več, glejte Kako narediti [popolno sinhronizacijo in poln uvoz v storitvi AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="4fe9b-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="4fe9b-122">**Imam težave s povezljivostjo z geslom nepotrjenim**</span><span class="sxs-lookup"><span data-stu-id="4fe9b-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="4fe9b-123">Prenesite in omogočite najnovejšo različico storitve [AZURE ad Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="4fe9b-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="4fe9b-124">Konfiguracija požarnega zidu: orodje za povezovanje v storitvi Azure AD (1.1.443 in zgoraj) bo moralo dostopati do programa **https** :</span><span class="sxs-lookup"><span data-stu-id="4fe9b-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="4fe9b-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4fe9b-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="4fe9b-126">servicebus. Windows. Networks</span><span class="sxs-lookup"><span data-stu-id="4fe9b-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="4fe9b-127">Dovoli nedejavne povezave, da trajajo vsaj 2-3 minut</span><span class="sxs-lookup"><span data-stu-id="4fe9b-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="4fe9b-128">**Še vedno imam težave z geslom nepotrjenim**</span><span class="sxs-lookup"><span data-stu-id="4fe9b-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="4fe9b-129">Če imate še vedno težave, poskusite onemogočiti in znova omogočiti storitev nepotrjenim gesel v orodju za povezovanje v storitvi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4fe9b-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="4fe9b-130">Če želite izvedeti več, glejte kako [onemogočiti in znova omogočiti nepotrjenim gesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="4fe9b-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
