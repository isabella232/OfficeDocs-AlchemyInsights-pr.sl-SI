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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506934"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogoči Office 365 napredno zaščito pred grožnjami za SharePoint online, OneDrive in Microsoft Teams

1. Pojdite na https://protection.office.com in se vpišite.
2. Izberite pravilnik za **upravljanje groženj**  >  **Policy**  >  **varne Priloge**.
3. Izberite **Vklopi ATP za SharePoint, OneDrive in Microsoft Teams**ter kliknite **Shrani**.
4. Priporočljivo Kot globalni skrbnik ali skrbnik SharePoint online zaženite ukaz [set-spot,](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet s parametrom **Disallowinfectedfiledownload** , ki je nastavljen na *True*.
5. Priporočljivo [Nastavite opozorila](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za odkrite datoteke.

> [!NOTE]
> ATP hoteti nČe želite skandirati sleherni posamezen pila v SharePoint online, OneDrive, ali mikroskop skupina. Datoteke skenirane asinhrono, skozi proces, ki uporablja skupno rabo in gostuje dogodki dejavnosti, skupaj s pametno hevristiko in grožnje signalov za prepoznavanje zlonamerne datoteke. Glejte [ATP za SharePoint, OneDrive in Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).