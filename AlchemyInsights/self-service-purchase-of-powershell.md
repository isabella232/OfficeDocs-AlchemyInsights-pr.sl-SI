---
title: Samopostrežni nakup lupine PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739986"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="7360b-102">Samopostrežni nakup lupine PowerShell</span><span class="sxs-lookup"><span data-stu-id="7360b-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="7360b-103">Če želite uporabiti modul PowerShell MSCommerce, ga morate namestiti v napravo s sistemom Windows 10 z TLS 1,2 (zahtevana je lokalna skrbniška dovoljenja).</span><span class="sxs-lookup"><span data-stu-id="7360b-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="7360b-104">Uvozite in povežite se z modulom MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="7360b-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="7360b-105">Ko ste pozvani k vpisu, boste morali uporabiti globalne poverilnice za skrbniško vlogo za obračunavanje.</span><span class="sxs-lookup"><span data-stu-id="7360b-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="7360b-106">Če nimate TLS 1,2, se lahko pri poskusu pridobivanja ali posodabljanja pravilnika prikaže to sporočilo o napaki:</span><span class="sxs-lookup"><span data-stu-id="7360b-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="7360b-107">*» ErrorMessage «– osnovna povezava je bila zaprta: Prišlo je do nepričakovane napake pri pošiljanju*.</span><span class="sxs-lookup"><span data-stu-id="7360b-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



