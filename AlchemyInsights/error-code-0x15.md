---
title: Koda napake 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Če prejmete sporočilo o napaki, medtem ko aktivirate Office 2013 za uvajanje oddaljenih namiznih storitev (RDS), razmislite o tem, kako omogočite knjižnice ADAL z urejanjem registra.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709203"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="9ac71-103">Napaka pri aktivaciji sistema Office 2013 v storitvah oddaljenega namizja</span><span class="sxs-lookup"><span data-stu-id="9ac71-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="9ac71-104">Če prejmete sporočilo o napaki, medtem ko aktivirate Office 2013 za uvajanje oddaljenih namiznih storitev (RDS), razmislite o tem, kako omogočite knjižnice ADAL z urejanjem registra.</span><span class="sxs-lookup"><span data-stu-id="9ac71-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="9ac71-105">**Registrski ključ**</span><span class="sxs-lookup"><span data-stu-id="9ac71-105">**Registry key**</span></span>|<span data-ttu-id="9ac71-106">**Vnesite**</span><span class="sxs-lookup"><span data-stu-id="9ac71-106">**Type**</span></span>|<span data-ttu-id="9ac71-107">**Vrednost**</span><span class="sxs-lookup"><span data-stu-id="9ac71-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9ac71-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="9ac71-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="9ac71-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="9ac71-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="9ac71-110">1</span><span class="sxs-lookup"><span data-stu-id="9ac71-110">1</span></span>  <br/> |

<span data-ttu-id="9ac71-111">Če želite več informacij, glejte [Omogočanje sodobnega preverjanja pristnosti za Office 2013 v napravah s sistemom Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="9ac71-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="9ac71-112">KNJIŽNICE ADAL je privzeto omogočen v programih Microsoft 365 za podjetja in Office 2016.</span><span class="sxs-lookup"><span data-stu-id="9ac71-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="9ac71-113">Oddaljenega namiznih storitev (RDS) je bilo prej imenovanih terminalskih storitev.</span><span class="sxs-lookup"><span data-stu-id="9ac71-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  