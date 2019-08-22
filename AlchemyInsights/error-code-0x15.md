---
title: Koda napake 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Če prejemate napake med aktiviranjem urad 2013 na uvajanje oddaljenega namizja storitve (RDS), menijo, ki omogoča ADAL z urejanjem registra.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527066"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="40668-103">Napaka pri aktiviranje Office 2013 na storitev oddaljenega namizja.</span><span class="sxs-lookup"><span data-stu-id="40668-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="40668-104">Če prejemate napake med aktiviranjem urad 2013 na uvajanje oddaljenega namizja storitve (RDS), menijo, ki omogoča ADAL z urejanjem registra.</span><span class="sxs-lookup"><span data-stu-id="40668-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="40668-105">**Registrski ključ**</span><span class="sxs-lookup"><span data-stu-id="40668-105">**Registry key**</span></span>|<span data-ttu-id="40668-106">**Vrsta**</span><span class="sxs-lookup"><span data-stu-id="40668-106">**Type**</span></span>|<span data-ttu-id="40668-107">**Vrednost**</span><span class="sxs-lookup"><span data-stu-id="40668-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="40668-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="40668-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="40668-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="40668-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="40668-110">1</span><span class="sxs-lookup"><span data-stu-id="40668-110">1</span></span>  <br/> |

<span data-ttu-id="40668-111">Če želite več informacij, glejte [Omogočajo sodobne preverjanje pristnosti za Office 2013 naprej okno načrt](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="40668-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="40668-112">FRENKX je privzeto omogočena v Office 365 ProPlus in Office 2016.</span><span class="sxs-lookup"><span data-stu-id="40668-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="40668-113">Oddaljenega namizja storitve (RDS) je bil prej imenovan terminalskih storitev.</span><span class="sxs-lookup"><span data-stu-id="40668-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  