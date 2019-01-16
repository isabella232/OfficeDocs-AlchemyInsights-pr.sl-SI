---
title: Koda napake 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Če prejemate napake med aktiviranjem urad 2013 na uvajanje oddaljenega namizja storitve (RDS), menijo, ki omogoča ADAL z urejanjem registra.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28312553"
---
<span data-ttu-id="df743-103">Če prejemate napake med aktiviranjem urad 2013 na uvajanje oddaljenega namizja storitve (RDS), menijo, ki omogoča ADAL z urejanjem registra.</span><span class="sxs-lookup"><span data-stu-id="df743-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="df743-104">**Registrski ključ**</span><span class="sxs-lookup"><span data-stu-id="df743-104">**Registry key**</span></span>|<span data-ttu-id="df743-105">**Vrsta**</span><span class="sxs-lookup"><span data-stu-id="df743-105">**Type**</span></span>|<span data-ttu-id="df743-106">**Vrednost**</span><span class="sxs-lookup"><span data-stu-id="df743-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="df743-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="df743-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="df743-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="df743-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="df743-109">1</span><span class="sxs-lookup"><span data-stu-id="df743-109">1</span></span>  <br/> |
   
<span data-ttu-id="df743-110">Če želite več informacij, glejte [Omogočajo sodobne preverjanje pristnosti za Office 2013 naprej okno načrt](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="df743-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="df743-p101">FRENKX je privzeto omogočena v Office 365 ProPlus in Office 2016. > Oddaljenega namizja storitve (RDS) je bil prej imenovan terminalskih storitev.</span><span class="sxs-lookup"><span data-stu-id="df743-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

