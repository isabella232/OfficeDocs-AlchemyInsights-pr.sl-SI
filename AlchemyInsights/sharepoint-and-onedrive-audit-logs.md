---
title: Poročila iz klasičnega SharePointovega dnevnika nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662224"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint in OneDrive dnevniki nadzora

## <a name="sharepoint-classic-audit-logs"></a>SharePoint Classic Audit dnevniki

SPO Legacy Audit je bil preseljen v poenoteni dnevnik nadzora (UAL). Vsa SPO podedovana poročila o nadzoru bodo zdaj napajana prek UAL, območni revizijski signali pa so preseljeni v UAL.

Ključne spremembe:

* Obrezovanje ni na voljo kot zmogljivost.
* Izbira določenih dogodkov za nadzor ni na voljo. Oglejte si [ta dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) za popoln seznam nadzorovanih dogodkov, ki so na voljo privzeto.
* Možnost» **mesto** «v razdelku» **poročila po meri** «ni na voljo.
* Možnost» **odpiranje ali prenos dokumentov** «ni na voljo.

[Konfiguracija nastavitev nadzora za zbirko mest](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint in OneDrive sodobni enotni dnevniki nadzora iz skladnosti

* [Vklop/izklop poenotenega pisanja dnevnika nadzora](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

V SharePointu ali OneDrive ni potrebna nobena dodatna konfiguracija.

Če želite preveriti dejavnost datotek, map (ov), uporabnikov (ov), dovoljenj:

* [Dejavnosti datoteke in strani](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Dejavnosti mape](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Dejavnosti zahteve za skupno rabo in dostop](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Dejavnosti sinhronizacije](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Dejavnosti skrbništva mesta](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Če želite več informacij o tem, kako pridobite te dogodke, si oglejte [iskanje dnevnika nadzora](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
