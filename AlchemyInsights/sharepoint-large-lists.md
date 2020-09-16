---
title: SharePointovi veliki seznami
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720149"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="078b3-102">Delo z velikimi seznami in knjižnicami v SharePointu</span><span class="sxs-lookup"><span data-stu-id="078b3-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="078b3-103">SharePointovi seznami in knjižnice lahko vsebujejo do 30.000.000 elementov, če pa imajo več kot 5.000 elementov, se lahko prikaže napaka praga pogleda seznama, ko poskušate delati z njimi.</span><span class="sxs-lookup"><span data-stu-id="078b3-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="078b3-104">Ta prag je v uporabi zaradi ohranjanja učinkovitosti delovanja storitve.</span><span class="sxs-lookup"><span data-stu-id="078b3-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="078b3-105">Praga ni mogoče spremeniti.</span><span class="sxs-lookup"><span data-stu-id="078b3-105">It can't be changed.</span></span> <span data-ttu-id="078b3-106">Če se želite izogniti hitting tega praga:</span><span class="sxs-lookup"><span data-stu-id="078b3-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="078b3-107">**Uporaba sodobne**</span><span class="sxs-lookup"><span data-stu-id="078b3-107">**Use modern**</span></span>

<span data-ttu-id="078b3-108">Pogledi, ki prikazujejo številne elemente, najbolje delujejo v sodobni izkušnji.</span><span class="sxs-lookup"><span data-stu-id="078b3-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="078b3-109">[Uporabite sodobno izkušnjo](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , da se izognete napakam, ki jih lahko vidite v klasični izkušnji.</span><span class="sxs-lookup"><span data-stu-id="078b3-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="078b3-110">**Dodajanje indeksov**</span><span class="sxs-lookup"><span data-stu-id="078b3-110">**Add indexes**</span></span>

<span data-ttu-id="078b3-111">Ko filtrirate ali razvrščate po stolpcu, ki nima indeksa, se bo morda prikazalo sporočilo o napaki.</span><span class="sxs-lookup"><span data-stu-id="078b3-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="078b3-112">Ročno [dodajte kazalo](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) iz **Nastavitev seznama** v meniju nastavitve in nato **Indeksirajte stolpce**.</span><span class="sxs-lookup"><span data-stu-id="078b3-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="078b3-113">**Urejanje pogleda seznama**</span><span class="sxs-lookup"><span data-stu-id="078b3-113">**Edit the list view**</span></span>

<span data-ttu-id="078b3-114">Če se pri delu z velikim seznamom pojavi napaka, [uredite pogled seznama](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="078b3-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="078b3-115">Te štiri spremembe bodo odpravile napake praga pogleda seznama.</span><span class="sxs-lookup"><span data-stu-id="078b3-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="078b3-116">Naredite vse štiri spremembe, da odstranite vse napake.</span><span class="sxs-lookup"><span data-stu-id="078b3-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="078b3-117">Če še vedno prihaja do napak, preverite [upravljanje velikih seznamov in knjižnic](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="078b3-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="078b3-118">Izberite **brez** od obojega, **ki je bilo najprej razvrščeno po stolpcu** , in **nato razvrstite po stolpcu**.</span><span class="sxs-lookup"><span data-stu-id="078b3-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="078b3-119">Izberite **brez** iz obeh **prve skupine po stolpcu** in **nato Združi po stolpcu**.</span><span class="sxs-lookup"><span data-stu-id="078b3-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="078b3-120">Izberite **brez** za vse stolpce v razdelku **vsote** .</span><span class="sxs-lookup"><span data-stu-id="078b3-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="078b3-121">Prekličite izbor vseh razen enega stolpca za prikaz iz razdelka **stolpci** .</span><span class="sxs-lookup"><span data-stu-id="078b3-121">Deselect all but one column for display from the **Columns** section.</span></span>

