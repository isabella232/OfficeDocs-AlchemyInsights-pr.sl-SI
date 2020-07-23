---
title: Odpravljanje težav s sinhronizacijo gesel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387893"
---
# <a name="troubleshoot-password-synchronization"></a>Odpravljanje težav s sinhronizacijo gesel

Če želite odpraviti težave s sinhronizacijo gesel, začnite z opravilom za odpravljanje težav aAD Connect, da ugotovite, zakaj se gesla ne sinhronizirajo. Če želite začeti, pojdite [na Upravljanje neposredne sinhronizacije](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Odprite novo sejo lupine Windows PowerShell v strežniku Azure AD Connect in izberite možnost **Zaženi kot** skrbnik.

2. Zaženite RemoteSigned Set-ExecutionPolicy ali Set-ExecutionPolicy neomejeno.

3. Zaženite čarovnika za povezavo Azure AD Connect.

4. Pojdite na stran Dodatna opravila > **Odpravljanje**  >  **težav .**

5. Izberite **Zaženi,** da odprete meni za odpravljanje težav z Lupino PowerShell.

6. Izberite **Odpravljanje težav s sinhronizacijo gesel**.

    Težava je po navadi, da geslo ni sinhronizirano za določen uporabniški račun.

    **Opombe** Sinhronizacija gesel ne uspe, če je bila zadnja uspešna sinhronizacija gesel pred časom.

Če želite več pomoči pri odpravljanju težav s sinhronizacijo gesel, glejte Odpravljanje težav s sinhronizacijo z [razhajanjem gesel s sinhronizacijo storitve Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).