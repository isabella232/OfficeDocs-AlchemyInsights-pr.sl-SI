---
title: Odpravljanje težav pri sinhronizaciji gesel
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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664942"
---
# <a name="troubleshoot-password-synchronization"></a>Odpravljanje težav pri sinhronizaciji gesel

Če želite odpraviti težave s sinhronizacijo gesel, začnite s tem opravilom za odpravljanje težav s povezovanjem napak, da ugotovite, zakaj se gesla ne sinhronizirajo. Če želite začeti, pojdite v razdelek [upravljanje neposredne sinhronizacije](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Odprite novo sejo sistema Windows PowerShell v strežniku Azure AD Connect Server in izberite možnost» **Zaženi kot skrbnik** «.

2. Zaženite Set-ExecutionPolicy RemoteSigned ali Set-ExecutionPolicy neomejena.

3. Zaženite čarovnika za povezovanje v storitvi Azure AD.

4. Pojdite na stran dodatna opravila > **Odpravljanje težav**  >  **naprej**.

5. Izberite» **Zaženi** «, da odprete meni odpravljanje težav z powershellom.

6. Izberite **Odpravljanje težav pri sinhronizaciji gesel**.

    Težava je običajno, da geslo ni sinhronizirano za določen uporabniški račun.

    **Opombe** Sinhronizacija gesel ni uspešna, če je bilo zadnje uspešno sinhronizirano geslo že nekaj časa nazaj.

Če želite več informacij o odpravljanju težav pri sinhronizaciji gesel, glejte [Odpravljanje težav z razprševanjem gesel s sinhronizacijo storitve AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).