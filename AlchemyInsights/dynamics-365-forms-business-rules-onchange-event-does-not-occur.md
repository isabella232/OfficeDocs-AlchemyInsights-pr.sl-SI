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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529035"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="a51fd-102">Dogodek OnChange se ne pojavi, če je polje programsko spremenjeno</span><span class="sxs-lookup"><span data-stu-id="a51fd-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="a51fd-103">Dogodek *OnChange* se ne pojavi, če je polje programsko spremenjeno z *atributom.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metoda.</span><span class="sxs-lookup"><span data-stu-id="a51fd-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="a51fd-104">Če želite, da se rutine za obravnavo dogodkov za dogodek *OnChange* zažene po tem, ko nastavite vrednost, morate uporabiti *atribut formcontext. data. entitet.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) način v kodi.</span><span class="sxs-lookup"><span data-stu-id="a51fd-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
