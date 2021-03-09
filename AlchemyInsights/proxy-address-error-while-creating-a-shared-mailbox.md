---
title: Napaka naslova strežnika proxy med ustvarjanjem nabiralnika v skupni rabi
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568306"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="6a65f-102">Napaka naslova strežnika proxy med ustvarjanjem nabiralnika ali drugega predmeta z omogočenimi e-poštnimi sporočili</span><span class="sxs-lookup"><span data-stu-id="6a65f-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="6a65f-103">Če ste poskusili ustvariti predmet z omogočeno e-pošto (nabiralnik, nabiralnik v skupni rabi itd.) in prejeli napako» naslov strežnika proxy» SMTP:alias@domain.com «je že uporabljen... «, je e-poštni naslov, ki ste ga izbrali, že sprejel drug predmet, ki je omogočen za e-pošto v vaši organizaciji.</span><span class="sxs-lookup"><span data-stu-id="6a65f-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="6a65f-104">Če želite poiskati uporabnika, skupino, nabiralnik v skupni rabi ali javno mapo, v kateri je ta e-poštni naslov in ga izbrisati ali spremeniti njegov e-poštni naslov.</span><span class="sxs-lookup"><span data-stu-id="6a65f-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="6a65f-105">Nato lahko ustvarite nov predmet z omogočenimi e-poštnimi sporočili, ki je na voljo v sproščenem e-poštnem naslovu.</span><span class="sxs-lookup"><span data-stu-id="6a65f-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="6a65f-106">Uporabite iskanje na domači strani, da jo poiščete.</span><span class="sxs-lookup"><span data-stu-id="6a65f-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="6a65f-107">Uporabite lahko tudi ta ukaz PowerShell za Exchange Online, da ga poiščete:</span><span class="sxs-lookup"><span data-stu-id="6a65f-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="6a65f-108">Če ne želite izbrisati obstoječega e-poštnega naslova, izberite nov e-poštni naslov novega predmeta, ki ga ustvarjate.</span><span class="sxs-lookup"><span data-stu-id="6a65f-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  