---
title: ADFS Federation certifikat poteče
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710423"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation certifikat poteče

Če želite odpraviti to težavo, sledite tem korakom:
  
1. Namestite modul Microsoft Azure Active Directory za lupino Windows PowerShell v računalniku (če modul še ni nameščen). Če želite to narediti, pojdite na [upravljanje programa AZURE ad z lupino Windows PowerShell](https://aka.ms/aadposh).

2. Sledite korakom v razdelku» scenarij 1: potekla je veljavnost potrdila za podpisovanje žetonov AD FS «» [prišlo je do napake pri dostopu do mesta «iz programa AD FS, ko se je združil uporabnik v Microsoft 365, Azure ali InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Sledite korakom v [posodobitvi ali popravite nastavitve federativne domene v Microsoft, Azure ali InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Če želite izvedeti več o podaljšanju potrdil federacije, glejte [obnovitev potrdil federacije za Microsoft 365 in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
