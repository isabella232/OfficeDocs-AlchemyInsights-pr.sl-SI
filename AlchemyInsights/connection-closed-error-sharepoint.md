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
ms.openlocfilehash: 0515ead28cdfdbdb9529c269b5170b294ab2b120
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543053"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="bc53f-102">Napaka »Temeljna povezava je bila zaprta« v SharePoint</span><span class="sxs-lookup"><span data-stu-id="bc53f-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="bc53f-103">Če prejemate napako »Temeljna povezava je bila zaprta« v programu SharePoint je morda povezana z zastarelim TLS-jem 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="bc53f-103">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="bc53f-104">Če želite več informacij, glejte te članke:</span><span class="sxs-lookup"><span data-stu-id="bc53f-104">For more info, see these articles:</span></span>

- [<span data-ttu-id="bc53f-105">Priprava na TLS 1.2 v Office 365 in Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="bc53f-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="bc53f-106">Če odjemalec nima podpore za TLS 1.2, pride do napak pri preverjanju pristnosti</span><span class="sxs-lookup"><span data-stu-id="bc53f-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="bc53f-107">Posodobitev, če želite omogočiti TLS 1.1 in TLS 1.2 kot privzete varne protokole v winhttp v Windows</span><span class="sxs-lookup"><span data-stu-id="bc53f-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="bc53f-108">Če so uporabniki na Windows 7, preverite, ali so preverjali [cipherne Windows TLS v Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)</span><span class="sxs-lookup"><span data-stu-id="bc53f-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>