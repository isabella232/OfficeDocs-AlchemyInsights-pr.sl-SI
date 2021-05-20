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
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539948"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Nepooblaščena napaka v SharePoint

Če se v programu SharePoint prikaže napaka »(401) Unauthorized«, je sporočilo morda povezano z zastarelo kodo TLS 1.0/1.1. Če želite več informacij, glejte:

- [Priprava na TLS 1.2 v Office 365 in Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Če odjemalec nima podpore za TLS 1.2, pride do napak pri preverjanju pristnosti](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Posodobitev, če želite omogočiti TLS 1.1 in TLS 1.2 kot privzete varne protokole v winhttp v Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Če so uporabniki na Windows 7, preverite, ali so preverjali [cipherne Windows TLS v Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)