---
title: DLP ne deluje po pričakovanjih
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707826"
---
# <a name="dlp-not-working-as-expected"></a>DLP ne deluje po pričakovanjih

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Nastavitev DLP**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** v sistemu Office 365 ne deluje po pričakovanjih? V tem primeru preverite, ali je **pravilnik za DLP** pravilno nastavljen in da podatki vsebujejo, kaj išče **pravilnik DLP** , ko ga ocenjujete.
  
Pravilniki DLP omogočajo prepoznavanje in zaščito občutljivih informacij v organizaciji. Če želite nastaviti pravilnike za DLP, uporabite informacije [tukaj](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **Katere pravilnike za DLP iščejo**
  
Ko uporabljate **vgrajene občutljive vrste podatkov** v centrih za varnost in skladnost, pravilniki DLP iščejo določene vzorce in elemente pri odkrivanju teh občutljivih vrst.
  
- **Vgrajene občutljive vrste informacij**

    Če želite več informacij o vgrajenih občutljivih vrstah in o tem, kaj išče pravilnik za DLP pri odkrivanju občutljive vrste, glejte: [Kaj iščejo vrste občutljivih informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Vrste občutljivih podatkov po meri**

    Če želite ustvariti občutljive vrste podatkov po meri, uporabite ta članek, če želite informacije o tem, kako ustvariti vrsto občutljivega po meri: [ustvarite vrsto občutljivih podatkov po meri](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Preskus pravilnika za DLP**

Če želite preskusiti podatke z vgrajenim tipom ali občutljivo vrsto podatkov po meri, uporabite možnost» **Vrsta preskusa** «v razdelku **razvrstitve**  >  **občutljive vrste informacij**. Če želite več informacij, glejte [preskušanje vrst občutljivih podatkov po meri](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Poročila**
  
- Pridobite občutljive vpoglede podatkov s [poročili DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Oglejte si natančne podrobnosti dogodka z [poročilom o incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
