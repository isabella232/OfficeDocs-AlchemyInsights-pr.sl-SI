---
title: 2491 opozorilo e-poštna sporočila iz "Phish Delivered zaradi najemnika ali uporabnika preglasijo" politika
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758950"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="e064f-102">Opozorilo e-poštna sporočila iz "Phish Delivered zaradi najemnika ali uporabnika preglasijo" politika</span><span class="sxs-lookup"><span data-stu-id="e064f-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="e064f-103">A ne izpolniti obveznosti buden zvitost imenovan "Phish Delivered zaradi najemnika ali uporabnik preglasitev" has been valjan jasno v najemniki s urad 365 ATP P1 ter P2 dati dovoljenje.</span><span class="sxs-lookup"><span data-stu-id="e064f-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="e064f-104">Če ste prejeli to opozorilo, tukaj so koraki za preiskavo:</span><span class="sxs-lookup"><span data-stu-id="e064f-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="e064f-105">V opozorilnem sporočilu kliknite **Ogled opozorila** , da greste na stran z **opozorili** v središču za skladnost varnostnega &.</span><span class="sxs-lookup"><span data-stu-id="e064f-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="e064f-106">Izberite opozorilo, da si ogledate možnost za **Ogled seznama sporočil** ali **Ogled sporočil v Raziskovalcu**.</span><span class="sxs-lookup"><span data-stu-id="e064f-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="e064f-107">Obe možnosti vas vključita v podrobnosti sporočila, ki vključuje ID sporočila.</span><span class="sxs-lookup"><span data-stu-id="e064f-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="e064f-108">Upoštevajte, da bo povezava raziskovalec groženj samodejno filtrirala sporočila, ki ustrezajo merilom opozoril.</span><span class="sxs-lookup"><span data-stu-id="e064f-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="e064f-109">Morda boste morali prilagoditi datumski filter v Raziskovalcu groženj.</span><span class="sxs-lookup"><span data-stu-id="e064f-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="e064f-110">Sporočilo o lažnem predstavljanju je bilo podano zaradi ročno konfiguriranega preglasitve:</span><span class="sxs-lookup"><span data-stu-id="e064f-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="e064f-111">Dovoljeni pošiljatelj ali domena, ki jo določi uporabnik.</span><span class="sxs-lookup"><span data-stu-id="e064f-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="e064f-112">Dovoljen pošiljatelj ali domena, ki jo je skrbnik nastavil v pravilnik za preprečevanje neželene pošte.</span><span class="sxs-lookup"><span data-stu-id="e064f-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="e064f-113">Dovoljen naslov IP v pravilniku filtra za povezavo.</span><span class="sxs-lookup"><span data-stu-id="e064f-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="e064f-114">Pravilo toka pošte (znano tudi kot pravilo prenosa), ki je konfigurirano za omogočanje sporočil.</span><span class="sxs-lookup"><span data-stu-id="e064f-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="e064f-115">Če menite, da je bilo sporočilo nepravilno označeno kot Phish, uporabite dodatek Outlookovega [poročila](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) za pošiljanje vzorcev sporočil Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e064f-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
