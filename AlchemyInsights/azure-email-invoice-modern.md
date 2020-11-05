---
title: Sodobna izdaja e-pošte v storitvi Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922144"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="af13f-102">E-poštno izdajanje računov v storitvi Azure</span><span class="sxs-lookup"><span data-stu-id="af13f-102">Email invoicing in Azure</span></span>

<span data-ttu-id="af13f-103">Če želite posodobiti svoj e-poštni račun, morate imeti vlogo lastnika ali sodelavca v profilu obračunavanja ali njegovem računu obračunavanja.</span><span class="sxs-lookup"><span data-stu-id="af13f-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="af13f-104">Ko se odločite, bodo vsi uporabniki z vlogami lastnika, plačnika, bralcev in upravitelja računov v profilu obračunavanja prejeli svoje račune v e-poštnem sporočilu.</span><span class="sxs-lookup"><span data-stu-id="af13f-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="af13f-105">Vpišite se v [portal Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="af13f-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="af13f-106">Poiščete **stroške Management + obračunavanje**.</span><span class="sxs-lookup"><span data-stu-id="af13f-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="af13f-107">Na levi strani izberite **računi** in nato na vrhu strani izberite **e-poštni račun** .</span><span class="sxs-lookup"><span data-stu-id="af13f-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="af13f-108">Če imate več profilov za obračunavanje, izberite profil obračunavanja in nato izberite **opt** in.</span><span class="sxs-lookup"><span data-stu-id="af13f-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="af13f-109">Izberite **Posodobi**.</span><span class="sxs-lookup"><span data-stu-id="af13f-109">Select **Update**.</span></span>
6. <span data-ttu-id="af13f-110">Če imate več profilov za obračunavanje, izberite profil obračunavanja in nato izberite **opt** in.</span><span class="sxs-lookup"><span data-stu-id="af13f-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="af13f-111">Drugim omogočite dostop do ogleda, prenosa in plačila računov tako, da dodelite vlogo upravitelja računov za profil obračunavanja MCA ali MPA.</span><span class="sxs-lookup"><span data-stu-id="af13f-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="af13f-112">Če ste se odločili, da dobite račun v e-pošti, bodo uporabniki prejeli tudi račune v e-pošti.</span><span class="sxs-lookup"><span data-stu-id="af13f-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="af13f-113">Vpišite se v [portal Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="af13f-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="af13f-114">Poiščete **stroške Management + obračunavanje**.</span><span class="sxs-lookup"><span data-stu-id="af13f-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="af13f-115">Izberite **profile obračunavanja** z leve strani.</span><span class="sxs-lookup"><span data-stu-id="af13f-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="af13f-116">Na seznamu profili obračunavanja izberite profil obračunavanja, za katerega želite dodeliti vlogo upravitelja računov.</span><span class="sxs-lookup"><span data-stu-id="af13f-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="af13f-117">Izberite **Access Control (iam)** na levi strani in nato na vrhu strani izberite **Dodaj** .</span><span class="sxs-lookup"><span data-stu-id="af13f-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="af13f-118">Na spustnem seznamu vloga izberite **Upravitelj računov**.</span><span class="sxs-lookup"><span data-stu-id="af13f-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="af13f-119">Vnesite e-poštni naslov uporabnika, ki mu želite omogočiti dostop.</span><span class="sxs-lookup"><span data-stu-id="af13f-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="af13f-120">Izberite **Shrani** , da dodelite vlogo.</span><span class="sxs-lookup"><span data-stu-id="af13f-120">Select **Save** to assign the role.</span></span>
