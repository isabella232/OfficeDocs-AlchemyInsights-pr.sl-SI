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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529035"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="1db52-102">Dogodek OnChange ne pride, če polja je spremenil programsko</span><span class="sxs-lookup"><span data-stu-id="1db52-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="1db52-103">Dogodek *OnChange* ne pride, če polje je spreminjate programsko na *atribut.* [NastaviVrednost](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metoda.</span><span class="sxs-lookup"><span data-stu-id="1db52-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="1db52-104">Če želite rutine za obravnavo dogodka za dogodek *OnChange* teči po nastavite vrednost, uporabite na *formContext.data.entity atributa.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metoda v kodi.</span><span class="sxs-lookup"><span data-stu-id="1db52-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
