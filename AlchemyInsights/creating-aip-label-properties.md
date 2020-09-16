---
title: Ustvarjanje pravilnikov AIP oznak
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732191"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="208ef-102">Ustvarjanje pravilnikov AIP oznak</span><span class="sxs-lookup"><span data-stu-id="208ef-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="208ef-103">Oznake za zaščito informacij Azure (AIP) je mogoče uporabiti s celotnim obsegom podatkov, ki jih organizacija običajno ustvari in shranjuje od najnižje razvrstitve osebnih podatkov do najvišje razvrstitve zelo zaupnih podatkov.</span><span class="sxs-lookup"><span data-stu-id="208ef-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="208ef-104">Pravilniki za zaščito informacij Azure veljajo za klasičnega odjemalca Azure Information Protection (AIP) in ne za  [odjemalca AIP Unified LabelY](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="208ef-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="208ef-105">Konfigurirate lahko več elementov v pravilniku AIP, vključno z možnostmi, kot so:</span><span class="sxs-lookup"><span data-stu-id="208ef-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="208ef-106">Možnost, za katero bo nalepka dovolila skrbnikom ali uporabnikom Razvrsti in zaščite (izbirno) dokumente in e-poštna sporočila</span><span class="sxs-lookup"><span data-stu-id="208ef-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="208ef-107">Možnost za uveljavljanje razvrstitve, ko uporabniki shranijo dokumente in pošljejo e-pošto</span><span class="sxs-lookup"><span data-stu-id="208ef-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="208ef-108">Možnost za samodejno označevanje e-poštnega sporočila, ki temelji na njenih prilogah.</span><span class="sxs-lookup"><span data-stu-id="208ef-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="208ef-109">Možnost nadzora nad tem, ali je vrstica za zaščito informacij prikazana v Officeovih programih</span><span class="sxs-lookup"><span data-stu-id="208ef-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="208ef-110">Če želite dodatne možnosti in informacije o pravilnikih o zaščiti informacij v storitvi Azure, glejte: [pregled pravilnika o varstvu podatkov Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="208ef-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="208ef-111">Za druge uporabne vire v zvezi s pravilniki o AIP si oglejte:</span><span class="sxs-lookup"><span data-stu-id="208ef-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="208ef-112">Vadnica: Konfiguracija nastavitev pravilnika za zaščito informacij Azure in ustvarjanje nove nalepke</span><span class="sxs-lookup"><span data-stu-id="208ef-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="208ef-113">Konfiguriranje pravilnika o varstvu podatkov Azure</span><span class="sxs-lookup"><span data-stu-id="208ef-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="208ef-114">Ustvarjanje in konfiguracija oznak občutljivosti in njihovih pravilnikov</span><span class="sxs-lookup"><span data-stu-id="208ef-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="208ef-115">Navodila za uporabo pogostih scenarijev, ki uporabljajo zaščito informacij v storitvi Azure</span><span class="sxs-lookup"><span data-stu-id="208ef-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="208ef-116">Pregled dokumentacije za zaščito informacij Azure</span><span class="sxs-lookup"><span data-stu-id="208ef-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="208ef-117">Zahteve za zaščito informacij Azure</span><span class="sxs-lookup"><span data-stu-id="208ef-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="208ef-118">Vadnica za hitri začetek za informacijsko zaščito Azure</span><span class="sxs-lookup"><span data-stu-id="208ef-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="208ef-119">Prenos odjemalca za zaščito informacij Azure</span><span class="sxs-lookup"><span data-stu-id="208ef-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)