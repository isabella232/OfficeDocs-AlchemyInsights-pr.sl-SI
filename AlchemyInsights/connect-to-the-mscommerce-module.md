---
title: Vzpostavljanje povezave z modulom MSCommerce
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
- "3528"
ms.openlocfilehash: 41dd044d99d14f25ea15699bfb74f7c37e3928c1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713254"
---
# <a name="connect-to-the-mscommerce-module"></a><span data-ttu-id="bb654-102">Vzpostavljanje povezave z modulom MSCommerce</span><span class="sxs-lookup"><span data-stu-id="bb654-102">Connect to the MSCommerce module</span></span>

<span data-ttu-id="bb654-103">Preden si lahko ogledate ali nastavite pravilnik AllowSelfServicePurchase, morate imeti vzpostavljeno povezavo z modulom MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="bb654-103">You must be connected to the MSCommerce module before you can view or set the AllowSelfServicePurchase policy.</span></span>  

<span data-ttu-id="bb654-104">Če želite vzpostaviti povezavo z modulom MSCommerce, v vrstici lupine PowerShell (PS C: \) vnesite ta ukaz:</span><span class="sxs-lookup"><span data-stu-id="bb654-104">To connect to the MSCommerce module, at the PowerShell prompt (PS C:\), enter the following command:</span></span>

`Connect-MSCommerce`

<span data-ttu-id="bb654-105">Odpre se pogovorno okno za vpis.</span><span class="sxs-lookup"><span data-stu-id="bb654-105">This will open a sign-in dialog.</span></span> <span data-ttu-id="bb654-106">Vnesite uporabniško ime in geslo za vpis.</span><span class="sxs-lookup"><span data-stu-id="bb654-106">Enter your username and password to sign-in.</span></span>

<span data-ttu-id="bb654-107">**Opomba:** &nbsp; &nbsp; Račun, ki se uporablja za vpis, mora biti podjetje ali skrbnik za obračunavanje.</span><span class="sxs-lookup"><span data-stu-id="bb654-107">**NOTE:**&nbsp;&nbsp;The account used to sign in must be a Company or Billing Administrator.</span></span>
