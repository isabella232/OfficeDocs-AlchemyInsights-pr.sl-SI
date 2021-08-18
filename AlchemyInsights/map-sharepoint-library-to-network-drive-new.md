---
title: Preslikava SharePoint knjižnice na omrežni pogon
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 4eae45992d3fe6b31ae4d1aed02484cf20cb2260
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315564"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>Preslikava SharePoint knjižnice na omrežni pogon

Namesto da presliknete omrežni pogon, sinhronizirajte SharePoint z novim odjemalcem sinhronizacija s storitvijo OneDrive, ki ponuja datoteke na zahtevo. Dostopajte do vseh svojih datotek v storitvi OneDrive brez uporabe lokalnega prostora v shrambi. Če želite več informacij, [glejte Sinhronizacija SharePoint in Teams](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) datotek z računalnikom in Shranjevanje prostora na disku s datotekami OneDrive na zahtevo za [Windows 10.](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)

Če ne želite uporabiti novega [](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)odjemalca za e-sinhronizacija s storitvijo OneDrive, ampak preslikati pogon, sledite tem korakom:

- [Odpravljanje težav s preslikanimi omrežnimi pogoni, ki se povežejo s SharePoint Onlineom](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [Do napak pri preverjanju pristnosti pride, če odjemalec nima podpore za TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**OPOMBA:** Če uporabljate Internet Explorer 10 s Windows 8 ali Windows 7 in je **dostop** zavrnjen  ali pot ni dostopna pri preslikavi pogona, to težavo odpravite tako, da namestite ta sprotni [popravek](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d).