---
title: Ni mogoče dostopati SharePoint skrbniškega središča OneDrive za Office
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
- "9001459"
- "5638"
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020460"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Ni mogoče dostopati SharePoint skrbniškega središča OneDrive za Office

- Če mesto skrbniškega središča za SharePoint ali OneDrive ni dostopno ali ni na voljo, je morda prišlo do začasne težave s storitvijo, pri kateri lahko uporabniki pride do začasnih zakasnitev ali napak pri krmarjenju, ko dostopajo do SharePoint mest ali OneDrive vsebine. Na nadzorni [plošči s stanjem](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) storitve preverite, ali je to vplivalo na vašo organizacijo.

- Globalni skrbniki in skrbniki storitve SharePoint morajo biti dodeljeni licenci storitve SharePoint. Pri novo ustvarjenih računih, ki jim je bila pravkar dodeljena licenca SharePoint ali vloga skrbnika, lahko pride do težav pri dostopu do storitve SharePoint, na primer »dostop zavrnjen« ali »uporabnika ni bilo mogoče najti«. Počakajte najmanj 24 ur, da bo sinhronizacija dokončana v vseh naših sistemih. Razumemo, da se 24 ur morda zdi zelo dolgo. V številnih primerih že delamo na rešitvi.

- Privileged Identity Management[(PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) uporabniki lahko prejmejo dostop zavrnjen, če je dovoljen časovni okvir za dostop zelo majhen, glejte Dostop je zavrnjen do računov [PIM.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)