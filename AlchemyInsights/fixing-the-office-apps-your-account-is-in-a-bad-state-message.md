---
title: Popravljanje aplikacij storitve Microsoft 365 Vaš račun je v slabem stanju
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812552"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="8ffa4-102">Odpravljanje napake »Vaš račun je v slabem stanju« v aplikacijah Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8ffa4-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="8ffa4-103">To napako odpravite tako, da v računalniku, v katerem to vpliva, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="8ffa4-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="8ffa4-104">Odprite Officeovo aplikacijo in izberite   >  **Datotečni**  >  **račun Odjavi se iz vseh računov.**</span><span class="sxs-lookup"><span data-stu-id="8ffa4-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="8ffa4-105">Znova se vpišite z uporabniškim računom z veljavno licenco.</span><span class="sxs-lookup"><span data-stu-id="8ffa4-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="8ffa4-106">Če želite podrobne informacije, glejte razdelek [Računi v Officeu](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="8ffa4-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="8ffa4-107">[Počistite poverilnice za Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic sistema Windows.</span><span class="sxs-lookup"><span data-stu-id="8ffa4-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="8ffa4-108">**Opomba:** Poti registra za Office 2016 so se spremenile v 16.0.</span><span class="sxs-lookup"><span data-stu-id="8ffa4-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="8ffa4-109">Primer: \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="8ffa4-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="8ffa4-110">Če pride do napake med vzpostavljanjem povezave s storitvijo Office 365 s storitvijo Office 2013, [omogočite sodobno preverjanje](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) pristnosti za Odjemalca za Office.</span><span class="sxs-lookup"><span data-stu-id="8ffa4-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="8ffa4-111">Če želite več informacij, glejte Odpravljanje težav z aplikacijami brez brskalnika, ki se ne morejo vpisati v [Microsoft 365, Azure ali Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="8ffa4-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

