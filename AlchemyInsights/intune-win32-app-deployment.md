---
title: InTune za uvajanje aplikacije Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461993"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="673ed-102">InTune za uvajanje aplikacije Win32</span><span class="sxs-lookup"><span data-stu-id="673ed-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="673ed-103">Microsoft InTune omogoča Win32 aplikacije, vključno z, vendar ne omejeno na MSI in. EXE je treba uvesti v naprave s sistemom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="673ed-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="673ed-104">Uporabljeni mehanizem za uvajanje zahteva, da je v ciljni napravi prisoten ukaz» InTune «(IME).</span><span class="sxs-lookup"><span data-stu-id="673ed-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="673ed-105">IME bo samodejno nameščeno zaradi usmerjanja skripta PowerShell ali uvedbe aplikacije Win32 v uporabnika/napravo.</span><span class="sxs-lookup"><span data-stu-id="673ed-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="673ed-106">Na voljo je tudi nabor predpogojev, ki jih je treba izpolniti, da se uvede Win32 aplikacije, ki vključujejo:</span><span class="sxs-lookup"><span data-stu-id="673ed-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="673ed-107">Podprte platforme: Windows 10 različica 1607 ali novejša (različica Enterprise, Pro in Education).</span><span class="sxs-lookup"><span data-stu-id="673ed-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="673ed-108">Podprta arhitektura: x86 in x64.</span><span class="sxs-lookup"><span data-stu-id="673ed-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="673ed-109">Upravljanje naprav:» ZVOČNa skupina «in» samodejno vpisan «(vključno s povezanimi hibridnimi domenami in samodejnim vpisom pravilnika skupine).</span><span class="sxs-lookup"><span data-stu-id="673ed-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="673ed-110">Oblika paketa aplikacije:. **intunewin**  datoteka, ki jo je pripravila [Orodja Microsoft Win32 Content prep](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="673ed-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="673ed-111">Omejitve</span><span class="sxs-lookup"><span data-stu-id="673ed-111">Limitations:</span></span>
    - <span data-ttu-id="673ed-112">Največja velikost: 8GB.</span><span class="sxs-lookup"><span data-stu-id="673ed-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="673ed-113">Nepodprta arhitektura: orožje.</span><span class="sxs-lookup"><span data-stu-id="673ed-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="673ed-114">Če želite informacije, povezane s temi koraki, preglejte dokument»[Dodaj, dodeli in spremljajte aplikacijo Win32 «v programu Microsoft InTune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add).</span><span class="sxs-lookup"><span data-stu-id="673ed-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="673ed-115">Podrobnosti o odpravljanju težav z uvajanjem programov v sistemu Windows, vključno z aplikacijami Win32, si lahko ogledate v teh dokumentih</span><span class="sxs-lookup"><span data-stu-id="673ed-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="673ed-116">Odpravljanje težav z namestitvijo aplikacije</span><span class="sxs-lookup"><span data-stu-id="673ed-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="673ed-117">Odpravljanje težav z Win32 programi</span><span class="sxs-lookup"><span data-stu-id="673ed-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)