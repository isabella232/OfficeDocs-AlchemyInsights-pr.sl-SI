---
title: Prenos storitev – premaknite vse storitve RDFE v drugo naročnino
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692177"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="3269d-102">Prenos storitev – premaknite vse storitve RDFE v drugo naročnino</span><span class="sxs-lookup"><span data-stu-id="3269d-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="3269d-103">**Premikanje virov**</span><span class="sxs-lookup"><span data-stu-id="3269d-103">**Move resources**</span></span>

<span data-ttu-id="3269d-104">Vire Azure lahko premaknete v drugo naročnino na Azure ali skupino virov pod isto naročnino z uporabo portala Azure, Azure PowerShell, Azure CLI ali ostali API za premikanje virov.</span><span class="sxs-lookup"><span data-stu-id="3269d-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="3269d-105">Preden lahko premikate vire, glejte:</span><span class="sxs-lookup"><span data-stu-id="3269d-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="3269d-106">Kontrolni seznam pred premikanjem virov</span><span class="sxs-lookup"><span data-stu-id="3269d-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="3269d-107">Storitve, ki jih je mogoče premakniti</span><span class="sxs-lookup"><span data-stu-id="3269d-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="3269d-108">Preverjanje veljavnosti selitve</span><span class="sxs-lookup"><span data-stu-id="3269d-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="3269d-109">Premikanje navodil za storitve</span><span class="sxs-lookup"><span data-stu-id="3269d-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="3269d-110">Če želite premakniti obstoječe vire v drugo skupino virov ali naročnino, lahko uporabite:</span><span class="sxs-lookup"><span data-stu-id="3269d-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="3269d-111">Portal Azure</span><span class="sxs-lookup"><span data-stu-id="3269d-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="3269d-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3269d-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="3269d-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="3269d-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="3269d-114">PREOSTALI API</span><span class="sxs-lookup"><span data-stu-id="3269d-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="3269d-115">Vadnica: [premikanje virov Azure v drugo skupino virov ali naročnino](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="3269d-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="3269d-116">**Odpravljanje napak v programu Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="3269d-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="3269d-117">Oglejte si spodnje članke, če želite izvedeti več o nekaterih pogostih napakah uvedbe Azure in prejemati informacije, da jih razrešite.</span><span class="sxs-lookup"><span data-stu-id="3269d-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="3269d-118">Če ne najdete kode napake pri uvedbi napake, glejte [Iskanje kode napake](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="3269d-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="3269d-119">Odpravljanje napak pri uvajanju</span><span class="sxs-lookup"><span data-stu-id="3269d-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="3269d-120">Odpravljanje težav s premikanjem virov Azure v novo skupino virov ali naročnino</span><span class="sxs-lookup"><span data-stu-id="3269d-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="3269d-121">Če želite nadgraditi naročnino na Azure, kot je na primer preklop iz brezplačnega plačila na as-you-go, boste morali pretvoriti naročnino.</span><span class="sxs-lookup"><span data-stu-id="3269d-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="3269d-122">Če želite nadgraditi brezplačno preskusno različico, si oglejte razdelek [Nadgradnja brezplačne preskusne različice ali naročnine na Microsoft Imagine Azure, da bo plačljiva](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="3269d-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="3269d-123">Če želite spremeniti račun» Plačaj kot vi-go «, glejte [Spreminjanje naročnine na vašo uporabo v storitvi Azure Pay – as-you-go](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="3269d-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="3269d-124">**Če želite dodati ali povezati naročnino na Azure za najemnika storitve Azure Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="3269d-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="3269d-125">Vpišite se in izberite naročnino, ki jo želite uporabiti, na strani» naročnine « [v portalu Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="3269d-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="3269d-126">Izberite **Spremeni imenik**.</span><span class="sxs-lookup"><span data-stu-id="3269d-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="3269d-127">Preglejte vsa opozorila, ki se prikažejo, nato pa izberite **Spremeni**.</span><span class="sxs-lookup"><span data-stu-id="3269d-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="3269d-128">Imenik je spremenjen za naročnino in prejeli boste sporočilo o uspehu.</span><span class="sxs-lookup"><span data-stu-id="3269d-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="3269d-129">Če se želite premakniti v nov imenik, uporabite preklopnik *imenika* .</span><span class="sxs-lookup"><span data-stu-id="3269d-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="3269d-130">Lahko traja do 10 minut, če želite, da se vse prikaže pravilno.</span><span class="sxs-lookup"><span data-stu-id="3269d-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="3269d-131">**Priporočeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="3269d-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="3269d-132">Prenos lastništva naročnine na Azure</span><span class="sxs-lookup"><span data-stu-id="3269d-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="3269d-133">Premikanje virov v novo skupino virov ali naročnino</span><span class="sxs-lookup"><span data-stu-id="3269d-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="3269d-134">Upravljanje virov z uporabo portala Azure</span><span class="sxs-lookup"><span data-stu-id="3269d-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
