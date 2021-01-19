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
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="91286-102">Odpravljanje težav s soglasjem uporabnika</span><span class="sxs-lookup"><span data-stu-id="91286-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="91286-103">Določite lahko, kako končni uporabniki soglašajo s programi prek portala Azure ali PowerShell.</span><span class="sxs-lookup"><span data-stu-id="91286-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="91286-104">Če želite več informacij, glejte [Nastavitve soglasja uporabnika](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .</span><span class="sxs-lookup"><span data-stu-id="91286-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="91286-105">Skrbnik lahko z API-jem za [Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) podeli soglasje za dodeljevanje dovoljenj v imenu posameznega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="91286-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="91286-106">Če želite več informacij, glejte [pridobi dostop v imenu uporabnika](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="91286-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="91286-107">[Napake](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)pri prijavi uporabnika: v tem članku so navedene napake, ki se lahko pojavijo med postopkom soglasja v programu.</span><span class="sxs-lookup"><span data-stu-id="91286-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="91286-108">Če odpravite težave z nepričakovanim privolitvijo, ki ne vsebujejo nobenih sporočil o napaki, glejte [scenariji preverjanja pristnosti za AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="91286-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>