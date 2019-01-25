---
title: Pretvarjanje nabiralnik uporabnika v nabiralnik v skupni rabi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29489740"
---
<span data-ttu-id="1e413-p101">Nabiralnik uporabnika lahko pretvorite samo v nabiralnik v skupni rabi če uporabnik ima licenco za izmenjavo. Ko se pretvori v nabiralnik, bo še naprej kažejo na seznamu aktivnih uporabnikov, ker ta seznam vključuje nabiralniki v skupni rabi. Pa pretvori nabiralnika bo tudi prikazal na seznamu nabiralnik v skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="1e413-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="1e413-p102">Če poskušate pretvoriti nabiralnik v Admin konzoli Exchange in pretvorba ne, vaš brskalnik predpomnilnik in piškotke in poskusite znova. Če to še vedno ne deluje, poskusite Pretvarjanje nabiralnik v programu Exchange Management Shell z tekmovanje v teku sledeč zapoved:</span><span class="sxs-lookup"><span data-stu-id="1e413-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="1e413-107">Več nabiralnik pretvorba informacij je na voljo v [spremeniti uporabniškega nabiralnika za nabiralnik v skupni rabi](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="1e413-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
