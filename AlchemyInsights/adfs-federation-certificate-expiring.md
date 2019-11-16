---
title: ADFS Federation certifikat poteče
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737205"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation certifikat poteče

Če želite odpraviti to težavo, sledite tem korakom:
  
1. Namestite modul Microsoft Azure Active Directory za lupino Windows PowerShell v računalniku (če modul še ni nameščen). Če želite to narediti, pojdite na [upravljanje programa AZURE ad z lupino Windows PowerShell](https://aka.ms/aadposh).

2. Sledite korakom v razdelku» scenarij 1: potekla je veljavnost potrdila za podpisovanje žetonov AD FS «iz [» prišlo je do napake pri dostopu do mesta «iz AD FS, ko se je Združeno uporabnik prijavil v Office 365, Azure ali InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Sledite korakom v [posodobitvi ali popravite nastavitve federirane domene v Officeu 365, Azure ali InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Če želite izvedeti več o podaljšanju potrdil federacije, glejte [obnovitev potrdil federacije za Office 365 in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
