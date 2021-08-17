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
ms.openlocfilehash: 04f56dfc7ebe7de91bc64a5e6d2b480b07741c6e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314364"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Nepooblaščena napaka v SharePoint

Če v programu SharePoint prejmete napako »(401) Unauthorized«, je sporočilo morda povezano z zastarelo kodo TLS 1.0/1.1. Če želite več informacij, glejte:

- [Priprava na TLS 1.2 v Office 365 in Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Če odjemalec nima podpore za TLS 1.2, pride do napak pri preverjanju pristnosti](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Posodobitev, če želite omogočiti TLS 1.1 in TLS 1.2 kot privzete varne protokole v winhttp v Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Če so uporabniki na Windows 7, preverite, ali so preverjali [cipherne Windows TLS v Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)