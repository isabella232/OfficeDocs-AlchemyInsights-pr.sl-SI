---
title: Odpravljanje težav s soglasjem uporabnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007914"
---
# <a name="troubleshoot-user-consent"></a>Odpravljanje težav s soglasjem uporabnika

1. Končni uporabniki se lahko s programi strinjajo prek portala Azure ali PowerShell. Če [želite več informacij, glejte](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) Nastavitve soglasja uporabnika.
1. Skrbnik lahko uporabi tudi Api za [Microsoft Graph za podelitev](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) soglasja za pooblaščena dovoljenja v imenu enega uporabnika. Če želite več informacij, [glejte Dobite dostop v imenu uporabnika.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Napake pri soglasju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)uporabnika: v tem članku so obravnavane napake, do katerih lahko pride med postopkom soglasja za aplikacijo. Če odpravljate nepričakovane pozive za soglasje, ki ne vsebujejo sporočil o napakah, glejte Scenariji [preverjanja pristnosti za Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)