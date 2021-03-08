---
title: Konfiguracija šifriranja sporočil za hibridno okolje
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526602"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="cdc7b-102">Konfiguracija šifriranja sporočil za hibridno okolje</span><span class="sxs-lookup"><span data-stu-id="cdc7b-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="cdc7b-103">Za hibridna Izmenjevalna okolja lahko uporabniki na mestu uporabe pošiljajo šifrirano e-pošto s šifriranjem Office Message encryption (OME) le, če je e-pošta usmerjena prek storitve Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="cdc7b-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="cdc7b-104">Če želite šifrirati e-poštna sporočila z uporabo OME, izvedite te korake:</span><span class="sxs-lookup"><span data-stu-id="cdc7b-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="cdc7b-105">S [čarovnikom za hibridne konfiguracije](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) lahko nastavite hibridno okolje.</span><span class="sxs-lookup"><span data-stu-id="cdc7b-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="cdc7b-106">Za nastavitev šifriranja ni potrebna nobena posebna navodila.</span><span class="sxs-lookup"><span data-stu-id="cdc7b-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="cdc7b-107">[Nastavite pravila za potek pošte za šifriranje,](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) kot jih običajno želite.</span><span class="sxs-lookup"><span data-stu-id="cdc7b-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


