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
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="eac51-102">Odpravljanje težav pri sinhronizaciji gesel</span><span class="sxs-lookup"><span data-stu-id="eac51-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="eac51-103">Če želite odpraviti težave s sinhronizacijo gesel, začnite s tem opravilom za odpravljanje težav s povezovanjem napak, da ugotovite, zakaj se gesla ne sinhronizirajo.</span><span class="sxs-lookup"><span data-stu-id="eac51-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="eac51-104">Če želite začeti, pojdite v razdelek [upravljanje neposredne sinhronizacije](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="eac51-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="eac51-105">Odprite novo sejo sistema Windows PowerShell v strežniku Azure AD Connect Server in izberite možnost» **Zaženi kot skrbnik** «.</span><span class="sxs-lookup"><span data-stu-id="eac51-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="eac51-106">Zaženite Set-ExecutionPolicy RemoteSigned ali Set-ExecutionPolicy neomejena.</span><span class="sxs-lookup"><span data-stu-id="eac51-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="eac51-107">Zaženite čarovnika za povezovanje v storitvi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eac51-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="eac51-108">Pojdite na stran dodatna opravila > **Odpravljanje težav**  >  **naprej**.</span><span class="sxs-lookup"><span data-stu-id="eac51-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="eac51-109">Izberite» **Zaženi** «, da odprete meni odpravljanje težav z powershellom.</span><span class="sxs-lookup"><span data-stu-id="eac51-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="eac51-110">Izberite **Odpravljanje težav pri sinhronizaciji gesel**.</span><span class="sxs-lookup"><span data-stu-id="eac51-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="eac51-111">Težava je običajno, da geslo ni sinhronizirano za določen uporabniški račun.</span><span class="sxs-lookup"><span data-stu-id="eac51-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="eac51-112">**Opombe** Sinhronizacija gesel ni uspešna, če je bilo zadnje uspešno sinhronizirano geslo že nekaj časa nazaj.</span><span class="sxs-lookup"><span data-stu-id="eac51-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="eac51-113">Če želite več informacij o odpravljanju težav pri sinhronizaciji gesel, glejte [Odpravljanje težav z razprševanjem gesel s sinhronizacijo storitve AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="eac51-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>