---
title: Težave z SharePoint v Windows 7 napravah
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125518"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Težave z SharePoint v Windows 7 napravah

Če prejmete napake v računalnikih Windows 7, medtem ko delate v SharePoint ali OneDrive, so lahko povezane z zastarelo uporabo TLS 1.0/1.1. Če želite več informacij, si oglejte:

- [Priprava na TLS 1.2 v Office 365 in Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 odjemalci morajo imeti omogočeno TLS1.2. Če želite več informacij, glejte [Do napak pri preverjanju pristnosti pride, če odjemalec nima podpore za TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Namestite KB3140245 in ustvarite vrednost registra. Če želite več informacij, glejte Posodobitev, da omogočite [TLS 1.1 in TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) kot privzete varne protokole v winhttp v Windows

- Windows 7 SP1/Windows 8 morajo imeti nameščene najnovejše cipherje TLS-jev. Če želite več informacij, [glejte Microsoftovo svetovanje glede varnosti 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


