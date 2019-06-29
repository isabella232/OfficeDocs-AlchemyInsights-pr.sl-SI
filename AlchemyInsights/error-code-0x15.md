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
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388261"
---
<span data-ttu-id="5da28-103">Če prejemate napake med aktiviranjem urad 2013 na uvajanje oddaljenega namizja storitve (RDS), menijo, ki omogoča ADAL z urejanjem registra.</span><span class="sxs-lookup"><span data-stu-id="5da28-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="5da28-104">**Registrski ključ**</span><span class="sxs-lookup"><span data-stu-id="5da28-104">**Registry key**</span></span>|<span data-ttu-id="5da28-105">**Vrsta**</span><span class="sxs-lookup"><span data-stu-id="5da28-105">**Type**</span></span>|<span data-ttu-id="5da28-106">**Vrednost**</span><span class="sxs-lookup"><span data-stu-id="5da28-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5da28-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="5da28-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="5da28-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="5da28-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="5da28-109">1</span><span class="sxs-lookup"><span data-stu-id="5da28-109">1</span></span>  <br/> |

<span data-ttu-id="5da28-110">Če želite več informacij, glejte [Omogočajo sodobne preverjanje pristnosti za Office 2013 naprej okno načrt](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="5da28-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="5da28-111">FRENKX je privzeto omogočena v Office 365 ProPlus in Office 2016.</span><span class="sxs-lookup"><span data-stu-id="5da28-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="5da28-112">> oddaljenega namizja storitve (RDS) je bil prej imenovan terminalskih storitev.</span><span class="sxs-lookup"><span data-stu-id="5da28-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  