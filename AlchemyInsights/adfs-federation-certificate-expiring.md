---
title: Potrdilo za povezovanje ADFS, ki poteče
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821967"
---
# <a name="adfs-federation-certificate-expiring"></a>Potrdilo za povezovanje ADFS, ki poteče

Če želite odpraviti to težavo, upoštevajte ta navodila:
  
1. V računalnik namestite modul Microsoft Azure Active Directory za Windows PowerShell (če modul še ni nameščen). Če želite to narediti, pojdite v [upravljanje imenika Azure AD z lupino Windows PowerShell.](https://aka.ms/aadposh)

2. Upoštevajte navodila v razdelku »1. primer: Potrdilo za podpisovanje žetonov AD FS je poteklo« v razdelku »Pri storitvi AD FS je prišlo do težave pri dostopu do mesta«, ko se zvezni uporabnik prijavi v [Microsoft 365, Azure ali Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Upoštevajte navodila v članku Posodobitev ali popravilo nastavitev domen v domeni [Microsoft, Azure ali Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Če želite izvedeti več o podaljšanju potrdil za povezovanje, glejte [Podaljšanje potrdil združevanja za Microsoft 365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)in Azure Active Directory.
