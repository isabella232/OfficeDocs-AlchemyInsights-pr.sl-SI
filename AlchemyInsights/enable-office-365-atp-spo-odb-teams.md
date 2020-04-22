---
title: Omogočanje sistema Office 365 ATP za SharePoint, OneDrive in Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703442"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogoči Office 365 napredno zaščito pred grožnjami za SharePoint online, OneDrive in Microsoft Teams

1. Pojdite na https://protection.office.com in se vpišite.
2. Izberite > **Policy**pravilnik > za **upravljanje groženj****varne Priloge**.
3. Izberite **Vklopi ATP za SharePoint, OneDrive in Microsoft Teams**ter kliknite **Shrani**.
4. Priporočljivo Kot globalni skrbnik ali skrbnik SharePoint online zaženite ukaz [set-spot,](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet s parametrom **Disallowinfectedfiledownload** , ki je nastavljen na *True*.
5. Priporočljivo [Nastavite opozorila](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za odkrite datoteke.

> [!NOTE]
> ATP hoteti nČe želite skandirati sleherni posamezen pila v SharePoint online, OneDrive, ali mikroskop skupina. Datoteke skenirane asinhrono, skozi proces, ki uporablja skupno rabo in gostuje dogodki dejavnosti, skupaj s pametno hevristiko in grožnje signalov za prepoznavanje zlonamerne datoteke. Glej [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams), Poglej.