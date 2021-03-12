---
title: Primer Microsoftovega pravilnika za preprečevanje lažnega predstavljanja za Microsoft Defender za Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750797"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="f7421-102">Primer Microsoftovega pravilnika za preprečevanje lažnega predstavljanja za Microsoft Defender za Office 365</span><span class="sxs-lookup"><span data-stu-id="f7421-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="f7421-103">Te nastavitve omogočajo pravilnik, imenovan *domena in izvršni direktor*.</span><span class="sxs-lookup"><span data-stu-id="f7421-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="f7421-104">Ta pravilnik zagotavlja zaščito uporabnika in domene pred poosebljanje, nato pa uporabi pravilnik za vse e-poštne pošte, ki jih prejmejo uporabniki v domeni.</span><span class="sxs-lookup"><span data-stu-id="f7421-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="f7421-105">Najprej dodajte te informacije, da ustvarite pravilnik:</span><span class="sxs-lookup"><span data-stu-id="f7421-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="f7421-106">**Ime**: domena in **Opis** CEO: zagotovite, da se direktor in vaša domena ne posnemata.</span><span class="sxs-lookup"><span data-stu-id="f7421-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="f7421-107">**Uporabljeno za**: izberite **domeno prejemnika**.</span><span class="sxs-lookup"><span data-stu-id="f7421-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="f7421-108">V razdelku **katero koli od teh** izberite **Izberi** in nato izberite domeno.</span><span class="sxs-lookup"><span data-stu-id="f7421-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="f7421-109">Izberite **+ Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="f7421-109">Select **+ Add**.</span></span> <span data-ttu-id="f7421-110">Potrdite potrditveno polje ob imenu domene na seznamu (na primer *contoso.com*), nato pa izberite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="f7421-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="f7421-111">Izberite **Dokončano**.</span><span class="sxs-lookup"><span data-stu-id="f7421-111">Select **Done**.</span></span>
- <span data-ttu-id="f7421-112">Ko je pravilnik ustvarjen, lahko prilagodite pravilnik tako, da uporabite te možnosti:</span><span class="sxs-lookup"><span data-stu-id="f7421-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="f7421-113">**Dodajanje uporabnikov za zaščito:** Za ta primer dodajte e-poštni naslov CEO na minimum.</span><span class="sxs-lookup"><span data-stu-id="f7421-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="f7421-114">**Dodajte domene za zaščito**: dodajte organizacijsko domeno, ki vključuje Office izvršnega direktorja.</span><span class="sxs-lookup"><span data-stu-id="f7421-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="f7421-115">**Izberite dejanja**: za **e-pošto, ki jo je poslal** lažni uporabnik, izberite **preusmeritev sporočila na drug e-poštni naslov**, nato pa vnesite e-poštni naslov varnostnega skrbnika (na primer *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="f7421-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="f7421-116">**Če je e-pošta poslana z** lažno domeno, izberite **karantena sporočila**.</span><span class="sxs-lookup"><span data-stu-id="f7421-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="f7421-117">**Inteligenca nabiralnika**: Ta možnost je privzeto izbrana, ko ustvarite nov pravilnik za preprečevanje lažnega predstavljanja.</span><span class="sxs-lookup"><span data-stu-id="f7421-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="f7421-118">To **Nastavitev pustite za najboljše** rezultate.</span><span class="sxs-lookup"><span data-stu-id="f7421-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="f7421-119">**Dodajanje zaupanja vrednih pošiljateljev in domen:** V tem primeru ne definirajte nobenega preglasitve.</span><span class="sxs-lookup"><span data-stu-id="f7421-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="f7421-120">Ko pregledate nastavitve, izberite **Ustvari to pravilnik** ali **Shrani**, kot je primerno.</span><span class="sxs-lookup"><span data-stu-id="f7421-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="f7421-121">Če želite izvedeti več, glejte [Pravilniki za preprečevanje lažnega predstavljanja v programu Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="f7421-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
