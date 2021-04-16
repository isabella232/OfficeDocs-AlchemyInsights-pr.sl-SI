---
title: Upravljanje globalnega seznama naslovov in adresarja brez povezave za organizacijo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794848"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="28f71-102">Upravljanje globalnega seznama naslovov (GAL) in adresarja brez povezave (OAB) za organizacijo</span><span class="sxs-lookup"><span data-stu-id="28f71-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="28f71-103">Globalni seznam naslovov (GAL) je seznam predmetov, ki podpirajo pošto (katerih koli prejemnikov, ki lahko prejmejo e-poštno sporočilo), v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="28f71-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="28f71-104">Seznam GAL je samodejno ustvarjen v vsaki organizaciji.</span><span class="sxs-lookup"><span data-stu-id="28f71-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="28f71-105">Če želite ločiti uporabnike po organizaciji ali lokaciji, lahko ustvarite dodatne sezname GAL, vendar lahko posamezni uporabniki prikažejo in uporabljajo le en seznam GAL hkrati.</span><span class="sxs-lookup"><span data-stu-id="28f71-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="28f71-106">Nekateri e-poštni odjemalci, kot je Outlook za Windows, prenesejo GAL za uporabo brez povezave.</span><span class="sxs-lookup"><span data-stu-id="28f71-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="28f71-107">To se imenuje adresar brez povezave (OAB).</span><span class="sxs-lookup"><span data-stu-id="28f71-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="28f71-108">V storitvi Exchange Online je adresar OAB posodobljen le vsakih 8 ur, nato pa ga morajo odjemalci prenesti ter posodobiti svoje lokalne kopije adresarja OAB.</span><span class="sxs-lookup"><span data-stu-id="28f71-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="28f71-109">Vsaka sprememba prejemnika mora biti najprej prikazana na seznamu GAL, da je lahko pozneje prenesena v adresar OAB.</span><span class="sxs-lookup"><span data-stu-id="28f71-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="28f71-110">Tukaj je nekaj splošno uporabljenih postopkov za seznam GAL in adresar OAB:</span><span class="sxs-lookup"><span data-stu-id="28f71-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="28f71-111">Zaradi različnih razlogov boste morda želeli skriti nekatere predmete na seznamu GAL.</span><span class="sxs-lookup"><span data-stu-id="28f71-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="28f71-112">Oglejte si [Skrivanje prejemnikov na seznamu naslovov](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="28f71-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="28f71-113">Če želite omogočiti določenim skupinam uporabnikov prilagojene poglede seznama GAL za organizacijo, glejte [Pravilniki adresarja v storitvi Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="28f71-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="28f71-114">Če želite [ustvariti globalni seznam naslovov v storitvi Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) ter pridobiti informacije o tem, kako uporabljati dovoljenja seznama GAL, glejte [Seznami naslovov v storitvi Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="28f71-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="28f71-115">Če ustvarite nove sezname GAL, boste morda želeli ustvariti tudi novi adresar OAB.</span><span class="sxs-lookup"><span data-stu-id="28f71-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="28f71-116">Glejte [Postopki adresarja brez povezave](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="28f71-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
