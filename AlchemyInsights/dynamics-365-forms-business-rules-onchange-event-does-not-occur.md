---
title: Dynamics 365 obrazci poslovna pravila – pravilo za podjetja, ki ne odpuščajo obrazca
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
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711507"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange dogodek se ne pojavi, če je polje spremenjeno programsko

Dogodek *OnChange* se ne pojavi, če je polje z *atributom* spremenjeno programsko. metoda [NastaviVrednost](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Če želite, da se za dogodek *OnChange* zaženejo rutina za obravnavo dogodkov, potem ko ste nastavili vrednost, morate uporabiti *atribut» formContext. data. entiteta* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) «v kodi.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
