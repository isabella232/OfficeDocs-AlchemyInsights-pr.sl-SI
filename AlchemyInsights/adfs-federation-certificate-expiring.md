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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952985"
---
# <a name="adfs-federation-certificate-expiring"></a>Potrdilo za povezovanje ADFS, ki poteče

Če želite odpraviti to težavo, upoštevajte ta navodila:
  
1. Namestite modul Microsoft Azure Active Directory za Windows PowerShell v računalnik (če modul še ni nameščen). Če želite to narediti, pojdite na [Upravljanje imenika Azure AD s Windows PowerShell](https://aka.ms/aadposh).

2. Upoštevajte navodila v razdelku »1. primer: Potrdilo za podpisovanje žetonov AD FS je poteklo« v razdelku »Prišlo je do težave pri dostopu do mesta« storitve AD FS, ko se zvezni uporabnik prijavi v Microsoft 365, Azure ali [Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Upoštevajte navodila v članku Posodobitev ali popravilo nastavitev domen v domeni [Microsoft, Azure ali Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Če želite izvedeti več o podaljšanju potrdil za povezovanje, [glejte Podaljšanje potrdil o združevanju za Microsoft 365 in Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
