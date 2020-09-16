---
title: 2491 opozoril e-poštnih sporočil iz pravilnika» Phish, ki je bil izdan zaradi najemnika ali preglasitve uporabnika «
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728627"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="8cdc6-102">Opozorilna e-poštna sporočila iz pravilnika» Phish, ki je bil izdan zaradi najemnika ali preglasitve uporabnika «</span><span class="sxs-lookup"><span data-stu-id="8cdc6-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="8cdc6-103">Privzeti pravilnik o opozorilih, imenovan» Phish dostavljena zaradi najemnika ali preglasitve uporabnika «, je bil razposlan v najemnike z licencami za Office 365 ATP P1 in P2.</span><span class="sxs-lookup"><span data-stu-id="8cdc6-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="8cdc6-104">Če ste prejeli to opozorilo, upoštevajte navodila za preiskavo:</span><span class="sxs-lookup"><span data-stu-id="8cdc6-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="8cdc6-105">V opozorilnem sporočilu kliknite **Ogled opozorila** , če se želite povrniti na stran **opozorila** v središču za skladnost varnostnega &.</span><span class="sxs-lookup"><span data-stu-id="8cdc6-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="8cdc6-106">Izberite opozorilo, da si ogledate možnost **ogleda seznama** sporočil ali **Ogled sporočil v Raziskovalcu**.</span><span class="sxs-lookup"><span data-stu-id="8cdc6-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="8cdc6-107">Obe možnosti bosta poskrbeli za podrobnosti sporočila, ki vključuje ID sporočila.</span><span class="sxs-lookup"><span data-stu-id="8cdc6-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="8cdc6-108">Povezava raziskovalca za grožnje samodejno filtrira sporočila, ki ustrezajo pogojem za opozorilo.</span><span class="sxs-lookup"><span data-stu-id="8cdc6-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="8cdc6-109">Morda boste morali prilagoditi datumski filter v Raziskovalcu grožnje.</span><span class="sxs-lookup"><span data-stu-id="8cdc6-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="8cdc6-110">Sporočilo o lažnem predstavljanju je bilo dostavljeno zaradi ročnega konfiguriranega preglasitve:</span><span class="sxs-lookup"><span data-stu-id="8cdc6-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="8cdc6-111">Dovoljen pošiljatelj ali domena, ki jo je nastavil uporabnik.</span><span class="sxs-lookup"><span data-stu-id="8cdc6-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="8cdc6-112">Dovoljen pošiljatelj ali domena, ki jo je nastavil skrbnik v pravilniku za preprečevanje neželene pošte.</span><span class="sxs-lookup"><span data-stu-id="8cdc6-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="8cdc6-113">Dovoljen naslov IP v pravilniku filtra povezave.</span><span class="sxs-lookup"><span data-stu-id="8cdc6-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="8cdc6-114">Pravilo poteka pošte (znano tudi kot pravilo prenosa), ki je konfigurirano tako, da dovoli sporočila.</span><span class="sxs-lookup"><span data-stu-id="8cdc6-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="8cdc6-115">Če menite, da je bilo sporočilo nepravilno označeno kot Phish, uporabite [dodatek Message Outlook Report](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) , da pošljete vzorce sporočil Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="8cdc6-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
