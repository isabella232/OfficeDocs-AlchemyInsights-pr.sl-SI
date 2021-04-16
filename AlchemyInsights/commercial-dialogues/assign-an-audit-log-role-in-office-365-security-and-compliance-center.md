---
title: Dodeljevanje vloge dnevnika nadzora v središču za skladnost z varnostnim &om sistema Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749523"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="1971e-102">Dodeljevanje vloge dnevnika nadzora v središču za skladnost z varnostnim &om sistema Office 365</span><span class="sxs-lookup"><span data-stu-id="1971e-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="1971e-103">Če želite poiskati dnevnik nadzora v storitvi Office 365, mora skrbnik dodeliti vlogo **dnevniki nadzora** , ki je le za ogled, in vlogo **dnevnika nadzora** v programu Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="1971e-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="1971e-104">Te vloge so privzeto dodeljene skupinam vlog za upravljanje skladnosti in upravljanje organizacije.</span><span class="sxs-lookup"><span data-stu-id="1971e-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="1971e-105">Globalni skrbniki v sistemu Office 365 in Microsoft 365 so samodejno dodani kot člani skupine vlog» Upravljanje organizacije «.</span><span class="sxs-lookup"><span data-stu-id="1971e-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="1971e-106">Če želite uporabniku omogočiti iskanje z minimalno ravnjo pravic, ustvarite skupino vlog po meri v storitvi Exchange Online, dodajte vlogo **dnevnika nadzora** , ki je le za  ogled, in nato dodajte uporabnika kot člana nove skupine vlog.</span><span class="sxs-lookup"><span data-stu-id="1971e-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="1971e-107">Če želite več informacij, glejte [Upravljanje skupin vlog v storitvi Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) in [iskanje dnevnika nadzora v središču za skladnost varnostnega &](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="1971e-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>