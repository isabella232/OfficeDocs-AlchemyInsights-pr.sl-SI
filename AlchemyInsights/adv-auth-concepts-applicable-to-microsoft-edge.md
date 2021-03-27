---
title: Koncepti naprednega preverjanja pristnosti, ki veljajo za Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398601"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="c35fc-102">Koncepti naprednega preverjanja pristnosti, ki veljajo za Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="c35fc-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="c35fc-103">Spodaj so napredna zasnova preverjanja pristnosti, ki veljajo za Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="c35fc-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="c35fc-104">**Proaktivno preverjanje pristnosti**</span><span class="sxs-lookup"><span data-stu-id="c35fc-104">**Proactive Authentication**</span></span>

<span data-ttu-id="c35fc-105">Ko omogočite pravilnik [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) bo Microsoft Edge poskusil proaktivno preveriti pristnost vpisanih uporabnikov prek Microsoftovih storitev.</span><span class="sxs-lookup"><span data-stu-id="c35fc-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="c35fc-106">V rednih intervalih bo spletna storitev preverjala, ali je na voljo posodobljen manifest, ki vsebuje konfiguracijo, ki urejajo proaktivno preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="c35fc-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="c35fc-107">Prednosti: Proaktivno preverjanje pristnosti omogoča preverjanje pristnosti za ključne storitve, kot je stran na novem zavihku »Office«.</span><span class="sxs-lookup"><span data-stu-id="c35fc-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="c35fc-108">Če kot iskalnik uporabljate Bing, proaktivno preverjanje pristnosti izboljša učinkovitost delovanja naslovne vrstice in pomaga ustvariti rezultate iskanja, prilagojene potrebam vašega podjetja.</span><span class="sxs-lookup"><span data-stu-id="c35fc-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="c35fc-109">**Windows Hello CredUI za preverjanje pristnosti NTLM**</span><span class="sxs-lookup"><span data-stu-id="c35fc-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="c35fc-110">Če enotna prijava (SSO) ni na voljo, ko se spletno mesto poskuša vpisati v uporabnika prek mehanizma NTLM ali Negotiate, ta funkcija omogoča uporabniku skupno rabo poverilnic operacijskega sistema s tem mestom in izpolnjevanje zahtev preverjanja pristnosti z uporabo uporabniškega vmesnika Windows Hello Cred UI.</span><span class="sxs-lookup"><span data-stu-id="c35fc-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="c35fc-111">Ta tok vpisa bo prikazan le v sistemu Windows 10 in le za uporabnike, ki med izzivom NTLM ali izzivom s pogajajo ne bodo dobili SSO.</span><span class="sxs-lookup"><span data-stu-id="c35fc-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="c35fc-112">**Samodejno vpisovanje s shranjenimi gesli**</span><span class="sxs-lookup"><span data-stu-id="c35fc-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="c35fc-113">Uporabniki, ki shranijo gesla v brskalniku Microsoft Edge, lahko omogočijo samodejni vpis na spletna mesta, kjer so shranili poverilnice.</span><span class="sxs-lookup"><span data-stu-id="c35fc-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="c35fc-114">Uporabniki lahko vklopijo ali izklopijo to funkcijo v edge://settings/passwords, lahko pa jo konfigurirate v [pravilnikih upravitelja](https://go.microsoft.com/fwlink/?linkid=2134622) gesel.</span><span class="sxs-lookup"><span data-stu-id="c35fc-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
