---
title: Dynamics 365 tvori poslovna pravila - pravila poslovanja, ni odpuščanja za obrazec
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748763"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Dogodek OnChange ne pride, če polja je spremenil programsko

Dogodek *OnChange* ne pride, če polje je spreminjate programsko na *atribut.* [NastaviVrednost](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metoda. Če želite rutine za obravnavo dogodka za dogodek *OnChange* teči po nastavite vrednost, uporabite na *formContext.data.entity atributa.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metoda v kodi.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
