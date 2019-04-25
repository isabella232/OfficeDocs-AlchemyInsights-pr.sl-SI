---
title: Koda napake 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Če prejemate napake med aktiviranjem urad 2013 na uvajanje oddaljenega namizja storitve (RDS), menijo, ki omogoča ADAL z urejanjem registra.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402755"
---
<span data-ttu-id="f032b-103">Če prejemate napake med aktiviranjem urad 2013 na uvajanje oddaljenega namizja storitve (RDS), menijo, ki omogoča ADAL z urejanjem registra.</span><span class="sxs-lookup"><span data-stu-id="f032b-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="f032b-104">**Registrski ključ**</span><span class="sxs-lookup"><span data-stu-id="f032b-104">**Registry key**</span></span>|<span data-ttu-id="f032b-105">**Vrsta**</span><span class="sxs-lookup"><span data-stu-id="f032b-105">**Type**</span></span>|<span data-ttu-id="f032b-106">**Vrednost**</span><span class="sxs-lookup"><span data-stu-id="f032b-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f032b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="f032b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="f032b-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="f032b-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="f032b-109">1</span><span class="sxs-lookup"><span data-stu-id="f032b-109">1</span></span>  <br/> |
   
<span data-ttu-id="f032b-110">Če želite več informacij, glejte [Omogočajo sodobne preverjanje pristnosti za Office 2013 naprej okno načrt](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="f032b-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="f032b-111">FRENKX je privzeto omogočena v Office 365 ProPlus in Office 2016.</span><span class="sxs-lookup"><span data-stu-id="f032b-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="f032b-112">> oddaljenega namizja storitve (RDS) je bil prej imenovan terminalskih storitev.</span><span class="sxs-lookup"><span data-stu-id="f032b-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

