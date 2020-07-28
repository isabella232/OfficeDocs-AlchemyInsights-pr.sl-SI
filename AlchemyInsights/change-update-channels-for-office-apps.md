---
title: Spreminjanje kanalov za posodabljanje za Officeove aplikacije
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440021"
---
# <a name="change-update-channels-for-office-apps"></a>Spreminjanje kanalov za posodabljanje za Officeove aplikacije

Če želite nove Officeove namestitve, z nastavitvami prenosa programske opreme za Office izberite želeni kanal za posodobitev in nato namestite (ali znova namestite) Officeove programe. Če želite več informacij, [glejte Upravljanje nastavitev prenosa programske opreme v storitvi Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

** Opomba** Kanal za posodabljanje, izbran z nastavitvami prenosa programske opreme za Office, velja za vse uporabnike, ki izvajajo nove namestitve prek portala O365. Če želite več informacij, [glejte Prenos in namestitev ali vnovična namestitev storitve Microsoft 365 ali Office 2019 v računalniku s sistemom Windows ali računalnik Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Če želite obstoječe officeove namestitve, uporabite Officeovo orodje za uvajanje (ODT), če želite preklopiti na drug kanal za posodabljanje:  

1. Prenesite najnovejšo različico Orodja za uvajanje Officea (setup.exe) iz Microsoftovega [centra za prenose](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Določite ime kanala, na katerem želite preklopiti. Če želite več informacij, [glejte Možnosti konfiguracije za Officeovo orodje za uvajanje](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Ustvarite konfiguracijsko datoteko XML, ki določa ustrezno ime kanala, na primer update.xml.  
    A. <Configuration>  
    B. <Posodobitve **Channel = "Mesečni"** />  
    C. </Configuration>
4. s visok zapoved uren, udarec s šibo v zgibalnik namestitev kraj setup.exe stolovati ter prost dostop sledeč zapoved:  
    A. setup.exe /configure update.xml
5. Zaženite Officeov program (na primer **File**Excel) in nato izberite  >  **Datotečni račun**. V razdelku Informacije o izdelku izberite **Posodobi možnosti**  >  **Posodobi zdaj**.

Če želite več informacij, [glejte Preklapljanje med kanali za posodabljanje obstoječih Officeovih programov](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Za preklapljanje med kanali za posodabljanje za izbrano skupino uporabnikov ali z upraviteljem konfiguracije (SCCM) konfigurirajte nastavitev Posodobi kanal z uporabo predmetnega pravilnika skupine. Če želite več informacij, [glejte Pregled kanalov za posodabljanje programov Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Če želite podrobnosti, [glejte Upravljanje kanalov Storitve Office 365 ProPlus](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) za profesionalce za IT in upravljanje [posodobitev za programe Microsoft 365 z Microsoft Endpoint Configuration Managerjem](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).