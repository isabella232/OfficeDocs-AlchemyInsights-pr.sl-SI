---
title: Enemu uporabniku je zavrnjen dostop med dodajanjem dodatkov v Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: ccb7af8477aba148ddc905448fa5a2b8bd1681443aa67865abfc69e1ca785f75
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54076145"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a>Enemu uporabniku je zavrnjen dostop med dodajanjem dodatkov v Outlook

Uporabnikov PowerShell Iskanje dovoljenj:

Get-ManagementRoleAssignment -RoleIgangnee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | Format-Table -Auto Role,Role ClarkgneeName,RolePilotgneeType