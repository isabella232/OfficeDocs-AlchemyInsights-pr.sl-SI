---
title: Apple MDM Push Certificate ni bil nastavljen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440010"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="af585-102">Apple MDM Push Certificate ni bil nastavljen</span><span class="sxs-lookup"><span data-stu-id="af585-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="af585-103">Apple MDM Push Certificate (znan tudi kot apple push notification service (APNS) ni bil konfiguriran za vašo naročnino.</span><span class="sxs-lookup"><span data-stu-id="af585-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="af585-104">Brez apple MDM Push certificate nastavljen, ne morete vpisati in upravljati iOS in Mac OS naprave.</span><span class="sxs-lookup"><span data-stu-id="af585-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="af585-105">Ko dodate potrdilo v intune, lahko uporabniki namestijo aplikacijo Portal podjetja, da včlanejo svoje naprave s sistemom iOS.</span><span class="sxs-lookup"><span data-stu-id="af585-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="af585-106">Izberite **"Strinjam se."**</span><span class="sxs-lookup"><span data-stu-id="af585-106">Select **"I agree."**</span></span> <span data-ttu-id="af585-107">dati Microsoftu dovoljenje za pošiljanje podatkov apple.</span><span class="sxs-lookup"><span data-stu-id="af585-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="af585-108">Izberite **Prenesite zahtevo za** podpisovanje potrdila za intune, ki je potrebna za ustvarjanje potisnega potrdila Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="af585-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="af585-109">Datoteka se uporablja za zahtevo certifikata odnosa zaupanja iz portala apple push certifikatov.</span><span class="sxs-lookup"><span data-stu-id="af585-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="af585-110">Izberite **Ustvari push potrdilo MDM, da** se poišate na portal apple push certifikatov.</span><span class="sxs-lookup"><span data-stu-id="af585-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="af585-111">Vpišite se s svojim podjetjem Apple ID in nato **izberite Ustvari potrdilo**.</span><span class="sxs-lookup"><span data-stu-id="af585-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="af585-112">Izberite **Izberi datoteko**, poiščite datoteko zahteve za podpisovanje certifikatov in nato **izberite Prenesi**.</span><span class="sxs-lookup"><span data-stu-id="af585-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="af585-113">Na strani Potrditev izberite **Prenesi,** da prenesete datoteko s potrdilom (.pem) in jo shranite lokalno.</span><span class="sxs-lookup"><span data-stu-id="af585-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="af585-114">**Opomba:** Potrdilo je povezano z APPLE ID-jem, ki se uporablja za njegovo ustvarjanje.</span><span class="sxs-lookup"><span data-stu-id="af585-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="af585-115">Za opravila upravljanja uporabite podjetje Apple ID in preverite, ali nabiralnik nadzoruje več oseb ali uporabljate seznam prejemnikov.</span><span class="sxs-lookup"><span data-stu-id="af585-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="af585-116">Nikoli ne uporabljajte osebnega Apple ID-ja.</span><span class="sxs-lookup"><span data-stu-id="af585-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="af585-117">Uporabite isti Apple ID obnoviti Apple Push certificate vsakih 12 mesecev.</span><span class="sxs-lookup"><span data-stu-id="af585-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="af585-118">Vnesite Apple ID, ki se uporablja za ustvarjanje push certifikata Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="af585-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="af585-119">Ta ID zasnemite kot opomnik za čas, ko morate obnoviti potrdilo.</span><span class="sxs-lookup"><span data-stu-id="af585-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="af585-120">Odprite datoteko s potrdilom (.pem), izberite **Odpri**in nato **Prenesi**.</span><span class="sxs-lookup"><span data-stu-id="af585-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="af585-121">S potisnim potrdilom lahko Intune vpiše in upravlja naprave Apple.</span><span class="sxs-lookup"><span data-stu-id="af585-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>