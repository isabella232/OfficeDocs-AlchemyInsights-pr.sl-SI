---
title: 401 Nepooblaščena napaka v SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233529"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Nepooblaščena napaka v SharePoint

Če se v programu SharePoint prikaže napaka »(401) Unauthorized«, je sporočilo morda povezano z zastarelo kodo TLS 1.0/1.1. Če želite več informacij, glejte:

[Priprava na TLS 1.2 v Office 365 in Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[Če odjemalec nima podpore za TLS 1.2, pride do napak pri preverjanju pristnosti](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Če so uporabniki na Windows 7, preverite, ali so preverjali [cipherne Windows TLS v Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)