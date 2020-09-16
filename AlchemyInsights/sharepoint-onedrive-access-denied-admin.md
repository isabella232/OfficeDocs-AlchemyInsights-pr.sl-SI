---
title: Odpravljanje težav z dostopom do zavrnjenih sporočil
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767679"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Odpravljanje težav z dostopom do sporočil v skrbniškem središču za SharePoint/OneDrive

Če prejmete sporočilo o zavrnjenem dostopu ob poskusu brskanja v skrbniškem središču za SharePoint/OneDrive, se prepričajte, da ste [uporabniku dodelili licenco](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Če ima uporabnik licenco, se prepričajte, da jim je [dodeljena skrbniška vloga](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , ki lahko dostopa do skrbniških centrov.

Do te težave lahko pride tudi, ko je uporabnik izbrisan in znova ustvarjen z istim glavnim imenom uporabnika (UPN). Nov račun je ustvarjen z uporabo drugega PUID (ID Passporta Unique). Ko uporabnik poskuša dostopati do zbirke mest ali njihove OneDrive, ima uporabnik nepravilen PUID. Drugi scenarij vključuje sinhronizacijo imenika z organizacijsko enoto imenika Active Directory (OU). Če so uporabniki že vpisani v SharePoint, nato pa so premaknjeni v drug OU in znova sinhronizirani s storitvijo SharePoint, lahko ta težava pride do te težave.

To težavo odpravite tako, da obnovite prvotni UPN s koraki v članku, [obnovite uporabnika v programu Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Opomba: Če v skrbniškem središču za OneDrive ali SharePoint ni na voljo več uporabnikov, ki so prej imeli dostop, je morda prišlo do začasne težave s storitvijo.  [Preverite nadzorno ploščo za stanje storitve](https://portal.office.com/adminportal/home#/servicehealth).


