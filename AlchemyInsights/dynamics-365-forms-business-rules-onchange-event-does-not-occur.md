---
title: Dynamics 365 obrazci poslovna pravila-pravilo poslovanja ne streljanje za obrazec
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769355"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="be495-102">Dogodek OnChange se ne pojavi, če je polje programsko spremenjeno</span><span class="sxs-lookup"><span data-stu-id="be495-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="be495-103">Dogodek *OnChange* se ne pojavi, če je polje programsko spremenjeno z *atributom.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metoda.</span><span class="sxs-lookup"><span data-stu-id="be495-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="be495-104">Če želite, da se rutine za obravnavo dogodkov za dogodek *OnChange* zažene, ko nastavite vrednost, morate v kodi [uporabiti metodo](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) *» formcontext. data. entiteta* «.</span><span class="sxs-lookup"><span data-stu-id="be495-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
