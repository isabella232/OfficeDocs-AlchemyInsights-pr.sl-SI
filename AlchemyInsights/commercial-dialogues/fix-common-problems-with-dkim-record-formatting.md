---
title: Odpravljanje pogostih težav z oblikovanjem zapisov DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930077"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Odpravljanje pogostih težav z oblikovanjem zapisov DKIM

Večina težav pri nastaviti DKIM je povezanih z nepravilnimi zapisi DNS.

Če želite odpraviti težave z nastaviti DKIM, preverite, ali je zapis DKIM CNAME **(ne** zapis TXT) pravilno oblikovan. Če želite več informacij, [glejte Kaj morate narediti, če želite ročno nastaviti DKIM v Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Če potrebujete pomoč za zapise DNS na splošno, glejte Ustvarjanje zapisov DNS pri poljubnih ponudnikih gostovanja DNS za [Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Ko ustvarite ali posodobite zapise DNS DKIM v storitvi gostovanja DNS za svojo domeno, boste morali počakati, da se zapisi DNS razširijo.
