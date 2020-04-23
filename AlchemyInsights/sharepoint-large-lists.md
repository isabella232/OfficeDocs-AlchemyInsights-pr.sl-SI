---
title: SharePointovi veliki seznami
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767301"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="851a4-102">Delo z velikimi seznami in knjižnicami v SharePointu</span><span class="sxs-lookup"><span data-stu-id="851a4-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="851a4-103">SharePointovi seznami in knjižnice lahko vsebujejo do 30.000.000 elementov, ko pa imajo več kot 5.000 elementov, se lahko pri poskusu dela z njimi prikaže napaka pri pogledu na seznam.</span><span class="sxs-lookup"><span data-stu-id="851a4-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="851a4-104">Ta prag je v uporabi zaradi ohranjanja učinkovitosti delovanja storitve.</span><span class="sxs-lookup"><span data-stu-id="851a4-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="851a4-105">Praga ni mogoče spremeniti.</span><span class="sxs-lookup"><span data-stu-id="851a4-105">It can't be changed.</span></span> <span data-ttu-id="851a4-106">Da bi se izognili hitting tega praga:</span><span class="sxs-lookup"><span data-stu-id="851a4-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="851a4-107">**Uporaba sodobnih**</span><span class="sxs-lookup"><span data-stu-id="851a4-107">**Use modern**</span></span>

<span data-ttu-id="851a4-108">Pogledi, ki prikazujejo veliko elementov, najbolje delujejo v sodobni izkušnji.</span><span class="sxs-lookup"><span data-stu-id="851a4-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="851a4-109">[Uporabite sodobno izkušnjo](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , da se izognete napakam, ki ste jih morda videli v klasični izkušnji.</span><span class="sxs-lookup"><span data-stu-id="851a4-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="851a4-110">**Dodajanje indeksov**</span><span class="sxs-lookup"><span data-stu-id="851a4-110">**Add indexes**</span></span>

<span data-ttu-id="851a4-111">Ko filtrirate ali razvrščate po stolpcu, ki nima kazala, se lahko prikaže sporočilo o napaki.</span><span class="sxs-lookup"><span data-stu-id="851a4-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="851a4-112">Ročno [dodajte indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) iz **Nastavitve seznama** v meniju z nastavitvami, nato **indeksirane stolpce**.</span><span class="sxs-lookup"><span data-stu-id="851a4-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="851a4-113">**Urejanje pogleda seznama**</span><span class="sxs-lookup"><span data-stu-id="851a4-113">**Edit the list view**</span></span>

<span data-ttu-id="851a4-114">Če pride do napake pri delu z velikim seznamom, [uredite pogled seznama](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="851a4-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="851a4-115">Naslednje štiri spremembe bodo odpravile napake praga pogleda seznama.</span><span class="sxs-lookup"><span data-stu-id="851a4-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="851a4-116">Naredite vse štiri spremembe, da odstranite vse napake.</span><span class="sxs-lookup"><span data-stu-id="851a4-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="851a4-117">Če še vedno dobivaš napake, preveri [upravljanje velikih seznamov in knjižnic](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="851a4-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="851a4-118">Izberite **brez** , tako **da jih najprej razvrstite po stolpcu** , **nato pa razvrstite po stolpcu**.</span><span class="sxs-lookup"><span data-stu-id="851a4-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="851a4-119">Izberite **brez** iz **prve skupine po stolpcu** in **nato združite po stolpcu**.</span><span class="sxs-lookup"><span data-stu-id="851a4-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="851a4-120">Za vse stolpce v odseku **vsote** izberite **brez** .</span><span class="sxs-lookup"><span data-stu-id="851a4-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="851a4-121">Počistite vse razen enega stolpca za prikaz iz odseka **stolpci** .</span><span class="sxs-lookup"><span data-stu-id="851a4-121">Deselect all but one column for display from the **Columns** section.</span></span>

