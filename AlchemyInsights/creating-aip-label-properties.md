---
title: Ustvarjanje pravilnikov o oznaki AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569512"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="28211-102">Ustvarjanje pravilnikov o oznaki AIP</span><span class="sxs-lookup"><span data-stu-id="28211-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="28211-103">Oznake za zaščito podatkov Azure (AIP) se lahko uporabljajo s celotnim obsegom podatkov, ki jih organizacija običajno ustvari in shranjuje, od najnižje razvrstitve osebnih podatkov do najvišje razvrstitve zelo zaupnih podatkov.</span><span class="sxs-lookup"><span data-stu-id="28211-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="28211-104">Pravilniki o varstvu podatkov Azure veljajo za klasični odjemalec za zaščito informacij Azure (AIP) in ne za [odjemalca AIP Unified označevanja](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="28211-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="28211-105">Konfigurirate lahko več elementov v pravilniku AIP, vključno z možnostmi, kot so:</span><span class="sxs-lookup"><span data-stu-id="28211-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="28211-106">Možnost, za katero bo oznaka dovolila skrbnikom ali uporabniku razvrščanje in zaščito (neobvezno) dokumentov in e-pošte</span><span class="sxs-lookup"><span data-stu-id="28211-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="28211-107">Možnost uveljavljanja razvrstitve, ko uporabniki shranijo dokumente in pošiljajo e-pošto</span><span class="sxs-lookup"><span data-stu-id="28211-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="28211-108">Možnost samodejnega označevanja e-poštnega sporočila na podlagi prilog.</span><span class="sxs-lookup"><span data-stu-id="28211-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="28211-109">Možnost nadzora nad tem, ali je vrstica za varstvo podatkov prikazana v Officeovih aplikacijah</span><span class="sxs-lookup"><span data-stu-id="28211-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="28211-110">Če želite dodatne možnosti in informacije o politikah za zaščito podatkov Azure, glejte: [pregled pravilnika o varstvu podatkov Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="28211-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="28211-111">Za druge koristne vire v zvezi s pravilniki AIP glejte:</span><span class="sxs-lookup"><span data-stu-id="28211-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="28211-112">Vadnica: Konfiguracija nastavitev pravilnika za zaščito podatkov Azure in ustvarjanje nove oznake</span><span class="sxs-lookup"><span data-stu-id="28211-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="28211-113">Konfiguriranje pravilnika o varstvu podatkov Azure</span><span class="sxs-lookup"><span data-stu-id="28211-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="28211-114">Ustvarjanje in konfiguriranje oznak občutljivosti in njihovih pravilnikov</span><span class="sxs-lookup"><span data-stu-id="28211-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="28211-115">Navodila za pogoste scenarije, ki uporabljajo Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="28211-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="28211-116">Preglejte dokumentacijo o varstvu podatkov Azure</span><span class="sxs-lookup"><span data-stu-id="28211-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="28211-117">Zahteve za zaščito podatkov Azure</span><span class="sxs-lookup"><span data-stu-id="28211-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="28211-118">Vodnik za hitri začetek za zaščito podatkov Azure</span><span class="sxs-lookup"><span data-stu-id="28211-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="28211-119">Prenesite odjemalca za zaščito podatkov Azure</span><span class="sxs-lookup"><span data-stu-id="28211-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)