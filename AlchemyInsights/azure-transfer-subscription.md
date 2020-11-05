---
title: Prenos lastništva za obračunavanje Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922170"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="27167-102">Prenos lastništva za obračunavanje Azure</span><span class="sxs-lookup"><span data-stu-id="27167-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="27167-103">Vpišite se v [portal Azure](https://portal.azure.com/) kot skrbnik računa obračunavanja, ki ima naročnino, ki jo želite prenesti.</span><span class="sxs-lookup"><span data-stu-id="27167-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="27167-104">Če niste prepričani, ali ste skrbnik ali če želite ugotoviti, kdo je, glejte [določanje skrbnika obračunavanja računov](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="27167-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="27167-105">Iskanje po **stroških upravljanja + obračunavanje**.</span><span class="sxs-lookup"><span data-stu-id="27167-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="27167-106">V levem podoknu izberite **naročnine** .</span><span class="sxs-lookup"><span data-stu-id="27167-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="27167-107">Odvisno od Accessa boste morda morali izbrati obseg obračunavanja **in nato naročnine** ali **Azure naročnine**.</span><span class="sxs-lookup"><span data-stu-id="27167-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="27167-108">Izberite» **prenos lastništva računa** «za naročnino, ki jo želite prenesti</span><span class="sxs-lookup"><span data-stu-id="27167-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="27167-109">Vnesite e-poštni naslov uporabnika, ki je skrbnik za obračunavanje računa, ki bo novi lastnik za naročnino, nato pa izberite **Pošlji zahtevo za prenos**</span><span class="sxs-lookup"><span data-stu-id="27167-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="27167-110">Uporabnik dobi e-poštno sporočilo z navodili za pregled zahteve za prenos.</span><span class="sxs-lookup"><span data-stu-id="27167-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="27167-111">Če želite odobriti zahtevo za prenos, uporabnik izbere povezavo v e-poštnem sporočilu in sledi navodilom.</span><span class="sxs-lookup"><span data-stu-id="27167-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="27167-112">**Opomba** : Če želite prenesti lastništvo nad naročnino na uporabniški račun v drugem najemniku storitve Azure ad, je treba trajno odstraniti vse naloge [nadzora dostopa, ki temeljijo na vlogi (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)za upravljanje virov v naročnini.</span><span class="sxs-lookup"><span data-stu-id="27167-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="27167-113">Le novi lastnik bo imel dostop do upravljanja virov v naročnini.</span><span class="sxs-lookup"><span data-stu-id="27167-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="27167-114">Če želite več informacij, glejte [prenos naročnine na uporabnika v drugem najemniku storitve AZURE ad](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="27167-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="27167-115">**Priporočeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="27167-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="27167-116">Prenos lastništva naročnine na storitev Azure na drug račun</span><span class="sxs-lookup"><span data-stu-id="27167-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="27167-117">O prenosu lastništva obračunavanja za naročnino na Azure</span><span class="sxs-lookup"><span data-stu-id="27167-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="27167-118">Prenos vizualnega studia, Microsoft partnerskega omrežja (MPN) in plačila po naročnini za dev/test</span><span class="sxs-lookup"><span data-stu-id="27167-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="27167-119">Pogosta vprašanja o prenosu lastništva</span><span class="sxs-lookup"><span data-stu-id="27167-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="27167-120">Odpravljanje težav pri prenosu lastništva</span><span class="sxs-lookup"><span data-stu-id="27167-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
