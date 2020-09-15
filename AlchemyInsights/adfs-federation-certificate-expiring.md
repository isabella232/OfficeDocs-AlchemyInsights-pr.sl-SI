---
title: Potrdilo o poteku ADFS federacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686766"
---
# <a name="adfs-federation-certificate-expiring"></a>Potrdilo o poteku ADFS federacije

Če želite odpraviti to težavo, upoštevajte ta navodila:
  
1. Namestite modul za Microsoft Azure Active Directory za Windows PowerShell v računalniku (če modul ni že nameščen). Če želite to narediti, pojdite na [Upravljanje storitve AZURE ad s sistemom Windows PowerShell](https://aka.ms/aadposh).

2. Upoštevajte navodila v razdelku» scenarij 1: potrdilo o vpisu v strežnik AD FS je poteklo «v razdelku» [prišlo je do težave pri dostopu do mesta «v storitvi AD FS, ko se Združeno uporabnik prijavi v Microsoft 365, Azure ali InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Upoštevajte navodila v [razdelku posodobitev ali popravljanje nastavitev Združenega domen v Microsoft, Azure ali InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Če želite izvedeti več o obnovitvi potrdil federacije, glejte [podaljšanje potrdil federacije za Microsoft 365 in imenik Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
