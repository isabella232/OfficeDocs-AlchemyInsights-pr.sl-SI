---
title: Odpravljanje težav s sporočili o zavrnjenem dostopu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085244"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Odpravljanje težav s sporočili o zavrnjenem dostopu v Skrbniškem središču za SharePoint/OneDrive

Če se vam je pri poskusu brskanja v Skrbniško središče za SharePoint/OneDrive prikaže sporočilo o zavrnjenem dostopu, se prepričajte, da ste uporabniku dodelili [licenco.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Če ima uporabnik licenco, se prepričajte tudi, da ima dodeljeno skrbniško [vlogo,](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ki ima dostop do skrbniških središč.

Do te težave lahko pride tudi, ko izbrišete uporabnika in ga znova ustvarite z istim glavnim imenom uporabnika (UPN). Novi račun je ustvarjen z drugo vrednostjo PUID (Passport Unique ID). Ko uporabnik poskuša dostopati do zbirke mest ali zbirke OneDrive, ima uporabnik napačen PUID. Drugi primer vključuje sinhronizacijo imenika z enoto organizacije imenika Active Directory (OU). Če so uporabniki že vpisani v SharePoint, nato pa so premaknjeni v drugo OU in znova sinhronizirani s SharePoint, lahko pride do te težave.

Če želite odpraviti to težavo, morate obnoviti izvirni UPN s koraki v članku Obnovitev [uporabnika v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Opomba: Če središče za OneDrive ali SharePoint ni na voljo več uporabnikom, ki so že imeli dostop, je morda prišlo do začasne težave s storitvijo.  [Preverite nadzorno ploščo s stanjem storitve.](https://portal.office.com/adminportal/home#/servicehealth)


