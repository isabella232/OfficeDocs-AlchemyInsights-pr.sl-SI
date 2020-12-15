---
title: Omogočanje upravljanja stroškov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678772"
---
# <a name="enable-cost-management"></a><span data-ttu-id="de4c8-102">Omogočanje upravljanja stroškov</span><span class="sxs-lookup"><span data-stu-id="de4c8-102">Enable cost management</span></span>

<span data-ttu-id="de4c8-103">**Kaj pomeni» stroški so onemogočeni za vašo organizacijo? «**</span><span class="sxs-lookup"><span data-stu-id="de4c8-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="de4c8-104">Organizacije, ki uporabljajo poslovne sporazume podjetja (EA) ali Microsoft Customer dogovore (MCA), lahko onemogočijo dostop do informacij o stroških in informacij o cenah.</span><span class="sxs-lookup"><span data-stu-id="de4c8-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="de4c8-105">Ko se prijavite v portal Azure, lahko uporabijo API-je za obračunavanje za programsko pridobivanje računov (ko se izberejo) in podrobnosti o uporabi.</span><span class="sxs-lookup"><span data-stu-id="de4c8-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="de4c8-106">**Kako omogočiti dodatnim uporabnikom dostop do računov**</span><span class="sxs-lookup"><span data-stu-id="de4c8-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="de4c8-107">Pojdite na **rezilo naročnine** na portalu Azure.</span><span class="sxs-lookup"><span data-stu-id="de4c8-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="de4c8-108">Izberite **računi** in nato **dostop do računov**.</span><span class="sxs-lookup"><span data-stu-id="de4c8-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="de4c8-109">Vklopite Access, nato pa shranite spremembe, da uporabnikom v naročnini, ki obsegajo vloge, omogočite prenos računov.</span><span class="sxs-lookup"><span data-stu-id="de4c8-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="de4c8-110">Skrbnik računa lahko konfigurira tudi račune, ki so poslani po e-pošti.</span><span class="sxs-lookup"><span data-stu-id="de4c8-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="de4c8-111">Če želite izvedeti več, glejte [pridobivanje računa v e-poštnem sporočilu](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="de4c8-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="de4c8-112">**Dodajanje uporabnikov v vlogo bralnika za obračunavanje**</span><span class="sxs-lookup"><span data-stu-id="de4c8-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="de4c8-113">Pojdite na **rezilo naročnine** na portalu Azure.</span><span class="sxs-lookup"><span data-stu-id="de4c8-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="de4c8-114">Izberite **Access Control (iam)** in nato kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="de4c8-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="de4c8-115">Izberite **bralnik obračunavanja** na strani **Izberite vlogo** .</span><span class="sxs-lookup"><span data-stu-id="de4c8-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="de4c8-116">Vnesite e-poštno sporočilo uporabnika, ki ga želite povabiti, in nato kliknite **v redu** , da pošljete povabilo.</span><span class="sxs-lookup"><span data-stu-id="de4c8-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="de4c8-117">Sledite navodilom, ki so na voljo v povabilu e-poštnega sporočila, da se prijavite kot bralnik obračunavanja.</span><span class="sxs-lookup"><span data-stu-id="de4c8-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="de4c8-118">Če želite več informacij, glejte [dodeljevanje dostopa do obračunavanja](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="de4c8-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="de4c8-119">**Priporočeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="de4c8-119">**Recommended documents**</span></span>

- [<span data-ttu-id="de4c8-120">Omogočanje pogledov» DA «in» AO «prek portala EA</span><span class="sxs-lookup"><span data-stu-id="de4c8-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="de4c8-121">Stroški, ki so vključeni v upravljanje stroškov</span><span class="sxs-lookup"><span data-stu-id="de4c8-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="de4c8-122">Podprte ponudbe za Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="de4c8-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="de4c8-123">Pregled stroškov v analizi stroškov</span><span class="sxs-lookup"><span data-stu-id="de4c8-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="de4c8-124">Omogočanje dostopa do informacij o obračunavanju</span><span class="sxs-lookup"><span data-stu-id="de4c8-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="de4c8-125">Preverjanje dostopa do Microsoftove pogodbe s strankami</span><span class="sxs-lookup"><span data-stu-id="de4c8-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






