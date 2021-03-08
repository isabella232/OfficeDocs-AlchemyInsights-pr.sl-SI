---
title: Odpravljanje pogostih težav z oblikovanjem zapisa DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525645"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="34f53-102">Odpravljanje pogostih težav z oblikovanjem zapisa DKIM</span><span class="sxs-lookup"><span data-stu-id="34f53-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="34f53-103">Večina težav z nastavitvijo DKIM se nanaša na nepravilne zapise DNS.</span><span class="sxs-lookup"><span data-stu-id="34f53-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="34f53-104">Če želite popraviti težave z nastavljanjem DKIM, preverite, ali je zapis CNAME DKIM (**ne** zapis txt) pravilno formatiran.</span><span class="sxs-lookup"><span data-stu-id="34f53-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="34f53-105">Če želite več informacij, glejte [Kaj morate narediti, če želite ročno NASTAVITI DKIM v storitvi Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="34f53-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="34f53-106">Če potrebujete pomoč za zapise DNS na splošno, si oglejte [Ustvarjanje zapisov DNS pri katerem koli ponudniku gostovanja DNS za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="34f53-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="34f53-107">Ko ustvarite ali posodobite zapise DNS DKIM pri ponudniku storitev gostovanja DNS za svojo domeno, boste morali počakati, da se zapisi DNS širijo.</span><span class="sxs-lookup"><span data-stu-id="34f53-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
