---
title: Omogočanje gesla writeback v storitvi Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560456"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="e218b-102">Omogočanje gesla writeback v storitvi Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e218b-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="e218b-103">Če želite omogočiti samopostrežno ponastavitev gesla writeback, najprej omogočite možnost writeback v storitvi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e218b-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="e218b-104">Iz strežnika Azure AD Connect Server dokončajte te korake:</span><span class="sxs-lookup"><span data-stu-id="e218b-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="e218b-105">Vpišite se v strežnik Azure AD Connect Server in zaženite čarovnika za konfiguracijo **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="e218b-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="e218b-106">Na **pozdravni** strani kliknite **Naprej**. </span><span class="sxs-lookup"><span data-stu-id="e218b-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="e218b-107">Na strani **dodatna opravila** izberite **prilagodite možnosti sinhronizacije** in nato kliknite **naprej**.</span><span class="sxs-lookup"><span data-stu-id="e218b-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="e218b-108">V **Povežite se s stranjo Azure AD**, vnesite poverilnico globalnega skrbnika za svojega najemnika Azure in nato kliknite **naslednja**.</span><span class="sxs-lookup"><span data-stu-id="e218b-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="e218b-109">V **povežite imenike** in **Domain/OU** filtrirajte strani, kliknite **naprej**.</span><span class="sxs-lookup"><span data-stu-id="e218b-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="e218b-110">Na strani **izbirne funkcije** potrdite polje ob možnosti **geslo writeback** in kliknite **naprej**.</span><span class="sxs-lookup"><span data-stu-id="e218b-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="e218b-111">Na strani **pripravljena** konfigurirati tako, da kliknete **Konfiguriraj** in počakate, da se postopek dokonča.</span><span class="sxs-lookup"><span data-stu-id="e218b-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="e218b-112">Ko vidite konfiguracijo Dokončaj, kliknite **Exit**.</span><span class="sxs-lookup"><span data-stu-id="e218b-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="e218b-113">Z geslom writeback omogočeno v storitvi Azure AD Connect, konfigurirajte Azure AD SSPR za writeback.</span><span class="sxs-lookup"><span data-stu-id="e218b-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="e218b-114">Če želite omogočiti geslo writeback v SSPR, dokončajte te korake:</span><span class="sxs-lookup"><span data-stu-id="e218b-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="e218b-115">Vpišite se v portal Azure z uporabo globalnega skrbniškega računa.</span><span class="sxs-lookup"><span data-stu-id="e218b-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="e218b-116">Poiščete in izberete **imenika Azure Active Directory**, kliknite **ponastavitev gesla**, nato pa kliknite **integracija na mestu uporabe**.</span><span class="sxs-lookup"><span data-stu-id="e218b-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="e218b-117">Nastavitev možnosti za **geslo za pisanje nazaj v imenik na mestu uporabe?** za **da**.</span><span class="sxs-lookup"><span data-stu-id="e218b-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="e218b-118">Nastavitev možnosti za **dovoli uporabnikom, da odklenejo račune, ne da bi morali ponastaviti svoje geslo?** za **da**.</span><span class="sxs-lookup"><span data-stu-id="e218b-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="e218b-119">Ko končate, kliknite **Dokončano**.</span><span class="sxs-lookup"><span data-stu-id="e218b-119">When ready, click **Save**.</span></span>

<span data-ttu-id="e218b-120">Če želite več informacij, glejte [omogočite samopostrežno ponastavitev gesla imenika Azure Active Directory, ki je na voljo v okolju na mestu uporabe,](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)writeback.</span><span class="sxs-lookup"><span data-stu-id="e218b-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="e218b-121">Ko skrbnik Ponastavi geslo uporabnika v portalu Azure, če je ta uporabnik povezan ali da je Razpršilo z geslom sinhronizirano, je geslo znova zapisano na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="e218b-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="e218b-122">Ta funkcija trenutno ni podprta v skrbniškem portalu za Office.</span><span class="sxs-lookup"><span data-stu-id="e218b-122">This functionality is currently not supported in the Office Admin portal.</span></span>