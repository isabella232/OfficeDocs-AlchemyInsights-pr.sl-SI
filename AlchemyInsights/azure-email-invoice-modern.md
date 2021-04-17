---
title: Sodobno izdajanje e-poštnih računov v storitvi Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820842"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="6024c-102">Izdajanje e-poštnih računov v storitvi Azure</span><span class="sxs-lookup"><span data-stu-id="6024c-102">Email invoicing in Azure</span></span>

<span data-ttu-id="6024c-103">Če želite posodobiti nastavitve izdajanja e-poštnih računov, morate imeti v profilu za obračunavanje ali v profilu za obračunavanje vlogo lastnika ali sodelavca.</span><span class="sxs-lookup"><span data-stu-id="6024c-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="6024c-104">Ko se odločite za sodelovanje, bodo vsi uporabniki, ki imajo vlogo lastnika, sodelavca, bralca in upravitelja računov v profilu za obračunavanje, prejeli svoj račun po e-pošti.</span><span class="sxs-lookup"><span data-stu-id="6024c-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="6024c-105">Vpišite se v [portal storitve Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="6024c-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="6024c-106">Poiščite **Upravljanje stroškov + obračunavanje**.</span><span class="sxs-lookup"><span data-stu-id="6024c-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="6024c-107">Na levi strani izberite možnost **Računi** in nato na vrhu strani **E-poštni račun**.</span><span class="sxs-lookup"><span data-stu-id="6024c-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="6024c-108">Če imate več profilov za obračunavanje, izberite profil za obračunavanje in izberite **Privolitev**.</span><span class="sxs-lookup"><span data-stu-id="6024c-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="6024c-109">Izberite **Posodobi**.</span><span class="sxs-lookup"><span data-stu-id="6024c-109">Select **Update**.</span></span>
6. <span data-ttu-id="6024c-110">Če imate več profilov za obračunavanje, izberite profil za obračunavanje in izberite **Privolitev**.</span><span class="sxs-lookup"><span data-stu-id="6024c-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="6024c-111">Drugim omogočite dostop do ogleda, prenosa in plačila računov tako, da jim dodelite vlogo upravitelja računa za profil za obračunavanje MCA ali MPA.</span><span class="sxs-lookup"><span data-stu-id="6024c-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="6024c-112">Če ste se odločili, da boste svoj račun prejeli po e-pošti, bodo tudi uporabniki prejeli račune po e-pošti.</span><span class="sxs-lookup"><span data-stu-id="6024c-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="6024c-113">Vpišite se v [portal storitve Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="6024c-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="6024c-114">Poiščite **Upravljanje stroškov + obračunavanje**.</span><span class="sxs-lookup"><span data-stu-id="6024c-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="6024c-115">Na levi strani izberite **Profili za obračunavanje**.</span><span class="sxs-lookup"><span data-stu-id="6024c-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="6024c-116">Na seznamu profilov obračunavanja izberite profil za obračunavanje, kateremu želite dodeliti vlogo upravitelja računov.</span><span class="sxs-lookup"><span data-stu-id="6024c-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="6024c-117">Na levi strani izberite možnost **Nadzor dostopa (IAM)** in nato na vrhu strani **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="6024c-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="6024c-118">Na spustnem seznamu vloge izberite **Upravitelj računov**.</span><span class="sxs-lookup"><span data-stu-id="6024c-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="6024c-119">Vnesite e-poštni naslov uporabnika, da dodelite dostop.</span><span class="sxs-lookup"><span data-stu-id="6024c-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="6024c-120">Izberite **Shrani**, da dodelite vlogo.</span><span class="sxs-lookup"><span data-stu-id="6024c-120">Select **Save** to assign the role.</span></span>
