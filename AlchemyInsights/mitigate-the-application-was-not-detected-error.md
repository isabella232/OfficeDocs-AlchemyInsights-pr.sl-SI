---
title: Odpravljanje napake »Aplikacije ni bilo mogoče odkriti«
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836367"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="eabd2-102">Odpravljanje napake »Aplikacije ni bilo mogoče odkriti«</span><span class="sxs-lookup"><span data-stu-id="eabd2-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="eabd2-103">Do napake pri namestitvi aplikacije, »Aplikacije ni bilo mogoče  odkriti po uspešno dokončani namestitvi,« ki se prikaže v programu Intune, lahko pride v vseh glavnih platformah OS (Windows, iOS in Android).</span><span class="sxs-lookup"><span data-stu-id="eabd2-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="eabd2-104">Najpogostejši scenariji, ki povzročijo to napako, vključujejo:</span><span class="sxs-lookup"><span data-stu-id="eabd2-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="eabd2-105">Program je bil po začetni uvedbi posodobljen zunaj programa Intune (iz trgovine z aplikacijami tretjih oseb).</span><span class="sxs-lookup"><span data-stu-id="eabd2-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="eabd2-106">Nekateri programi, na primer, kot je Google Chrome, lahko izvedejo samodejne posodobitve.</span><span class="sxs-lookup"><span data-stu-id="eabd2-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="eabd2-107">Uporabnik je odstranil aplikacijo po prvotni namestitvi.</span><span class="sxs-lookup"><span data-stu-id="eabd2-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="eabd2-108">Če želite to težavo ublažiti, najprej opravite pregled prizadetih naprav, da določite scenarij, v katerem pride do napake.</span><span class="sxs-lookup"><span data-stu-id="eabd2-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="eabd2-109">Če je bil program posodobljen zunaj programa Intune, je uvedba programa lahko nastavljena tako, da prezre različico aplikacije.</span><span class="sxs-lookup"><span data-stu-id="eabd2-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="eabd2-110">To naredite tako, da v razdelku **Konfiguracija aplikacije > Informacije o aplikaciji** nastavite različico **Prezri aplikacijo** v **Da**.</span><span class="sxs-lookup"><span data-stu-id="eabd2-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="eabd2-111">Pri ciljanju na stranko je morda primerno, da aplikacijo namestite kot je »zahtevano«, in tako zagotovite, da bo uvedena najnovejša različica.</span><span class="sxs-lookup"><span data-stu-id="eabd2-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="eabd2-112">Druga možnost je, da v platformi iOS uporabite **funkcijo samodejnega posodabljanja**, ki je povezana s programom za količinski nakup Apple, ki ga lahko konfigurirate tako, da bo samodejno posodabljal nove različice aplikacij, ko bodo na voljo.</span><span class="sxs-lookup"><span data-stu-id="eabd2-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="eabd2-113">Če želite več informacij o odpravljanju težav z namestitvijo aplikacije, si oglejte [Odpravljanje težav z namestitvijo aplikacije](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="eabd2-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
