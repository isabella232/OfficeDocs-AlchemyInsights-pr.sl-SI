---
title: Pravila za podjetja storitve Dynamics 365 Forms – poslovno pravilo se ne obžiga v obrazcu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947315"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Dogodek OnChange se ne zgodi, če se polje programsko spremeni

Dogodek *OnChange* se ne zgodi, če se polje programsko spremeni z *atributom.* [nastavi MetodoVrednost.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Če želite, da se rutine za obravnavo dogodkov za dogodek *OnChange* zaženejo, ko nastavite vrednost, morate v kodi uporabiti metodo *formContext.data.entity* [fireOpreme.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
