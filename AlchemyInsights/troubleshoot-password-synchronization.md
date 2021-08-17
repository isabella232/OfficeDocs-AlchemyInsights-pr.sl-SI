---
title: Odpravljanje težav s sinhronizacijo gesel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105774"
---
# <a name="troubleshoot-password-synchronization"></a>Odpravljanje težav s sinhronizacijo gesel

Če želite odpraviti težave s sinhronizacijo gesel, začnite s tem orodjem AAD in Povezovalnik, da ugotovite, zakaj se gesla ne sinhronizirajo. Za začetek pojdite na [Upravljanje neposredne sinhronizacije.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Odprite novo sejo Windows PowerShell v strežniku Azure AD Povezovalnik in izberite **možnost Zaženi kot** skrbnik.

2. Zaženite Set-ExecutionPolicy RemoteSigned ali Set-ExecutionPolicy Neomejeno.

3. Zaženite čarovnika za Povezovalnik Azure AD.

4. Pojdite na stran Dodatna opravila in > **odpravljanje**  >  **težav naprej.**

5. Izberite **Zaženi,** da odprete meni za odpravljanje težav z lupino PowerShell.

6. Izberite Odpravljanje **težav s sinhronizacijo gesel.**

    Običajno je težava v tem, da geslo ni sinhronizirano za določen uporabniški račun.

    **Opombe** Sinhronizacija gesla ne uspe, če je bila zadnja uspešna sinhronizacija gesla pred časom pred časom.

Če želite več pomoči pri odpravljanju težav s sinhronizacijo gesel, glejte Odpravljanje težav s sinhronizacijo gesla [s sinhronizacijo Povezovalnik z geslom.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)