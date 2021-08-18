---
title: Officea ni mogoče aktivirati
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: a057aaa2ddf8885b96c0fe0d5fa87d3a1b191af9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327862"
---
# <a name="unable-to-activate-office"></a>Officea ni mogoče aktivirati

**Opomba:** Če uporabljate starejšo različico programa Windows (na primer Windows 7), se prepričajte, da je TLS 1.2 omogočen kot privzeta različica. Če želite več informacij, glejte Posodobitev, da [omogočite TLS 1.1 in TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kot privzete varne protokole v winhttp v storitvi Windows.

- Preverite, ali je stanje naročnine poteklo.
- Prepričajte se, da imate naročnino, ki omogoča odjemalske licence, na primer Office 365 Business ali Business Premium in [se prepričajte, da je uporabniku dodeljena licenca](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Prepričajte se, da se uporabnik vpisuje v Office z računom, za katerega je dodeljena licenca.
- Oglejte si [stran z ustreznostjo stanja storitve Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) in preverite, ali obstajajo znane težave s storitvijo.
- Preverite požarni zid, protivirusni program in nastavitve proxyja ter se prepričajte, da ne blokirajo dostopa Microsoft 365 aplikacij v internetu. Glejte [URL-je in obsege naslovov IP za Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL-ji in razponi naslovov IP za Office 365").

**Namig** na računalnikih s sistemom Windows lahko diagnosticirate in samodejno odpravite več pogostih težav pri vpisu v Office. Prenesite in zaženite orodje **[Pomočnik za podporo in obnovitev](https://aka.ms/SaRA-OfficeSignInScenario)** za uporabo avtomatiziranega orodja.

Upoštevajte ta dejanja za odpravljanje težav:

- Odprite Officeovo aplikacijo in se [izpišite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) iz obstoječega uporabniškega računa. [Odstranite](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) licenco za Office in jo [znova dodelite](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users), nato pa se [vpišite v Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) z uporabniškim računom, s katerim imate težave.
- Zaženite [orodje za odpravljanje težav z aktiviranjem](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Ponastavite stanje aktiviranja Officea](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Ponastavite stanje aktiviranja Officea")
- [Izvedite spletno popravilo Officea](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Za dodatne rešitve odpravljanja težav glejte:  

- [Napake v Officeu, povezane z nelicenciranim izdelkom in aktiviranjem](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Pri aktiviranju Officea se prikaže napaka »Povezave z vašim računom ni mogoče vzpostaviti. Poskusite znova pozneje«](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)