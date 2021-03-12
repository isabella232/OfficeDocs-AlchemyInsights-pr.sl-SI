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
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Dodeljevanje vloge dnevnika nadzora v središču za skladnost z varnostnim &om sistema Office 365

Če želite poiskati dnevnik nadzora v storitvi Office 365, mora skrbnik dodeliti vlogo **dnevniki nadzora** , ki je le za ogled, in vlogo **dnevnika nadzora** v programu Exchange Online. Te vloge so privzeto dodeljene skupinam vlog za upravljanje skladnosti in upravljanje organizacije. Globalni skrbniki v sistemu Office 365 in Microsoft 365 so samodejno dodani kot člani skupine vlog» Upravljanje organizacije «.

Če želite uporabniku omogočiti iskanje z minimalno ravnjo pravic, ustvarite skupino vlog po meri v storitvi Exchange Online, dodajte vlogo **dnevnika nadzora** , ki je le za  ogled, in nato dodajte uporabnika kot člana nove skupine vlog.

Če želite več informacij, glejte [Upravljanje skupin vlog v storitvi Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) in [iskanje dnevnika nadzora v središču za skladnost varnostnega &](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).