---
title: ADF federacije potrdilo poteče
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
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499907"
---
# <a name="adfs-federation-certificate-expiring"></a>ADF federacije potrdilo poteče

Če želite odpraviti to težavo, sledite tem korakom:
  
1. Namestitev na Microsoft Azure Active Directory Module for Windows PowerShell v računalniku (če je modul ni že nameščen). Uganjati to, pojdite na [upravljanje Azure AD z lupino Windows PowerShell](https://aka.ms/aadposh).

2. Sledite korakom v je "scenarij 1: AD FS žeton podpisno potrdilo poteklo" oddelek [»Ni bilo problem dostop do strani« napaka iz AD FS, ko zunanji uporabnik prijavi v Office 365, Azure, ali Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Sledite korakom kako [posodobite ali popravite nastavitve združeno domeno v Office 365, Azure, ali Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).

    Če želite izvedeti več o podaljšanju federacije potrdila, glej [Obnovi federacije potrdila za Office 365 in Azure storitve Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
