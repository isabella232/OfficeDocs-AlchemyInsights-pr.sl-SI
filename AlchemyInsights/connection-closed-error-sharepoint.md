---
title: Temeljna povezava je bila zaprta v SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: f0f82eaaa00d71992af445bb89346fb85bad3ade5d120b25ad3a6ea4f9674893
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883335"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Napaka »Temeljna povezava je bila zaprta« v SharePoint

Če prejemate napako »Temeljna povezava je bila zaprta« v programu SharePoint je morda povezana z zastarelim TLS-jem 1.0/1.1. Če želite več informacij, glejte te članke:

- [Priprava na TLS 1.2 v Office 365 in Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Če odjemalec nima podpore za TLS 1.2, pride do napak pri preverjanju pristnosti](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Posodobitev, če želite omogočiti TLS 1.1 in TLS 1.2 kot privzete varne protokole v winhttp v Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Če so uporabniki na Windows 7, preverite, ali so preverjali [cipherne Windows TLS v Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)