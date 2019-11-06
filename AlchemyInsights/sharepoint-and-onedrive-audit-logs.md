---
title: Poročila o klasičnem SharePointovem dnevniku revizij
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992634"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Dnevniki revizij v SharePointu in storitvi OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Dnevniki klasičnih revizij v SharePointu

Revizija SPO je bila preseljena v dnevnik poenotenega nadzora (UAL). Vsa podedovana revizijska poročila SPO se bodo zdaj napajala prek UAL, podedovani revizijski signali pa so bili preseljeni v UAL.

Ključne spremembe:

* Obrezovanje ni na voljo kot zmožnost.
* Izbiranje specifičnih dogodkov za revizijo ni na voljo. Za celoten seznam revidiranih dogodkov, ki so privzeto na voljo, glejte [ta dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) .
* Možnost **lokacija** pod **prilagojena poročila** ni na voljo.
* Možnosti **odpiranja ali prenosa dokumentov** ni na voljo.

[Konfiguracija nastavitev revizij za zbirko mest](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Iz skladnosti se dnevniki programa SharePoint in OneDrive Modern Unified Audit

* [Vklop/izklop pisanja dnevnika poenotenega nadzora](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

V SharePointu ali storitvi OneDrive ni potrebna nobena dodatna konfiguracija.

Uporaba iskanja dnevnika nadzora za preverjanje dejavnosti datotek, map, uporabnikov, dovoljenj:

* [Dejavnosti datotek in strani](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Dejavnosti mape](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Skupna raba in dostop do dejavnosti zahteve](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Dejavnosti sinhronizacije](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Dejavnosti upravljanja spletnega mesta](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Če želite več informacij o tem, kako pridobite te dogodke, glejte [iskanje dnevnika revizij](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
