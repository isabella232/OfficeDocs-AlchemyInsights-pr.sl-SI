---
title: Pretvarjanje nabiralnik uporabnika v nabiralnik v skupni rabi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496451"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="9cb99-102">Spremeniti uporabnik poštni nabiralnik v nabiralnik v skupni rabi</span><span class="sxs-lookup"><span data-stu-id="9cb99-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="9cb99-103">Nabiralnik uporabnika lahko pretvorite samo v nabiralnik v skupni rabi če uporabnik ima licenco za izmenjavo.</span><span class="sxs-lookup"><span data-stu-id="9cb99-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="9cb99-104">Ko se pretvori v nabiralnik, bo še naprej kažejo na seznamu aktivnih uporabnikov, ker ta seznam vključuje nabiralniki v skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="9cb99-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="9cb99-105">Pa pretvori nabiralnika bo tudi prikazal na seznamu nabiralnik v skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="9cb99-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="9cb99-106">Če poskušate pretvoriti nabiralnik v Admin konzoli Exchange in pretvorba ne, vaš brskalnik predpomnilnik in piškotke in poskusite znova.</span><span class="sxs-lookup"><span data-stu-id="9cb99-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="9cb99-107">Če to še vedno ne deluje, poskusite Pretvarjanje nabiralnik v programu Exchange Management Shell z tekmovanje v teku sledeč zapoved:</span><span class="sxs-lookup"><span data-stu-id="9cb99-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="9cb99-108">Več nabiralnik pretvorba informacij je na voljo v [spremeniti uporabniškega nabiralnika za nabiralnik v skupni rabi](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="9cb99-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
