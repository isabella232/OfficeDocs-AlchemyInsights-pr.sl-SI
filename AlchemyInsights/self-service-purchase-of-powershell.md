---
title: Samopostrežna nakup PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091765"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="63462-102">Samopostrežna nakup PowerShell</span><span class="sxs-lookup"><span data-stu-id="63462-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="63462-103">Če želite uporabiti modul MSCommerce PowerShell, ga morate namestiti v napravo s sistemom Windows 10 s TLS 1,2 (zahtevana lokalna skrbniška dovoljenja).</span><span class="sxs-lookup"><span data-stu-id="63462-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="63462-104">Uvozite in povežite se z modulom MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="63462-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="63462-105">Ko se prikaže poziv za prijavo, boste morali uporabiti poverilnice globalnega skrbnika ali vloge za obračunavanje.</span><span class="sxs-lookup"><span data-stu-id="63462-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="63462-106">Če nimate TLS 1,2, se lahko pri poskusu posodobitve pravilnika prikaže ta napaka:</span><span class="sxs-lookup"><span data-stu-id="63462-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="63462-107">*ErrorMessage-osnovna povezava je bila zaprta: pri pošiljanju je prišlo do nepričakovane napake*.</span><span class="sxs-lookup"><span data-stu-id="63462-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



