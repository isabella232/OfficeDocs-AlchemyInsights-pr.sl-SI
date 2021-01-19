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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901629"
---
# <a name="troubleshoot-user-consent"></a>Odpravljanje težav s soglasjem uporabnika

1. Določite lahko, kako končni uporabniki soglašajo s programi prek portala Azure ali PowerShell. Če želite več informacij, glejte [Nastavitve soglasja uporabnika](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .
1. Skrbnik lahko z API-jem za [Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) podeli soglasje za dodeljevanje dovoljenj v imenu posameznega uporabnika. Če želite več informacij, glejte [pridobi dostop v imenu uporabnika](https://docs.microsoft.com/graph/auth-v2-user).
1. [Napake](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)pri prijavi uporabnika: v tem članku so navedene napake, ki se lahko pojavijo med postopkom soglasja v programu. Če odpravite težave z nepričakovanim privolitvijo, ki ne vsebujejo nobenih sporočil o napaki, glejte [scenariji preverjanja pristnosti za AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).