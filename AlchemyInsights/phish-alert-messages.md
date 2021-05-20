---
title: 2491 – Opozori e-poštna sporočila s pravilnika »Dostavljena phish zaradi najemnika ali preglasitve uporabnika«
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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544594"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="6e81e-102">Pravilnik »Opozorilo o e-poštnih sporočilih, dostavljene zaradi najemnika ali preglasitve uporabnika«</span><span class="sxs-lookup"><span data-stu-id="6e81e-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="6e81e-103">Privzeti pravilnik za opozorila z imenom »Ažuga, dostavljen zaradi najemnika ali preglasitve uporabnika« je bil izstavljen najemnikom za licence za Office 365 P1 in P2.</span><span class="sxs-lookup"><span data-stu-id="6e81e-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="6e81e-104">Če ste prejeli to opozorilo, si spodaj spodaj korakih raziščite:</span><span class="sxs-lookup"><span data-stu-id="6e81e-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="6e81e-105">V sporočilu z opozorilom kliknite **Ogled** opozorila, da se odpre **stran** Opozorila v središču za & s predpisi.</span><span class="sxs-lookup"><span data-stu-id="6e81e-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="6e81e-106">Če si želite ogledati možnost Ogled seznama **sporočil ali Ogled sporočil** v **Raziskovalcu, izberite opozorilo.**</span><span class="sxs-lookup"><span data-stu-id="6e81e-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="6e81e-107">Obe možnosti se prikažeta do podrobnosti sporočila, ki vključuje ID sporočila.</span><span class="sxs-lookup"><span data-stu-id="6e81e-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="6e81e-108">Povezava Raziskovalca groženj samodejno filtrira sporočila, ki ustrezajo pogojem opozorila.</span><span class="sxs-lookup"><span data-stu-id="6e81e-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="6e81e-109">Morda boste morali prilagoditi datumski filter v Raziskovalcu groženj.</span><span class="sxs-lookup"><span data-stu-id="6e81e-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="6e81e-110">Sporočilo z lažnim predstavljanjem je bilo dostavljeno zaradi ročno konfigurirane preglasitve:</span><span class="sxs-lookup"><span data-stu-id="6e81e-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="6e81e-111">Dovoljenih pošiljateljev ali domen, ki jih je nastavil uporabnik.</span><span class="sxs-lookup"><span data-stu-id="6e81e-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="6e81e-112">Dovoljenih pošiljateljev ali domen, ki jih je nastavil skrbnik v pravilniku za preprečevanje neželene pošte.</span><span class="sxs-lookup"><span data-stu-id="6e81e-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="6e81e-113">Dovoljeni naslov IP v pravilniku filtra povezave.</span><span class="sxs-lookup"><span data-stu-id="6e81e-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="6e81e-114">Pravilo toka pošte (znano tudi kot prenosno pravilo), ki je konfigurirano tako, da omogoča sporočila.</span><span class="sxs-lookup"><span data-stu-id="6e81e-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="6e81e-115">Če mislite, da je bilo sporočilo nepravilno označeno kot [](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) »phish« in želite poslati vzorce sporočil Microsoftu, Outlook »Poročilo o sporočilu«.</span><span class="sxs-lookup"><span data-stu-id="6e81e-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
