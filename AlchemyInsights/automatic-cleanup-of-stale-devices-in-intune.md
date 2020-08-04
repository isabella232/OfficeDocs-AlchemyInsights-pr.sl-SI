---
title: Samodejno čiščenje zastarelih naprav v intunu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555734"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="1704a-102">Samodejno čiščenje zastarelih naprav v intunu</span><span class="sxs-lookup"><span data-stu-id="1704a-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="1704a-103">Intune omogoča admin nastaviti časovni interval med 90 in 270 dni, po katerem zastarele naprave so odstranjene iz storitve.</span><span class="sxs-lookup"><span data-stu-id="1704a-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="1704a-104">Ta nastavitev je organizacija na stežaj in ko je aktivirana začne veljati takoj.</span><span class="sxs-lookup"><span data-stu-id="1704a-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="1704a-105">Vse naprave, ki niso bile prijavljene v strežnik Intune za obdobje, ki presega nastavitev, se trajno izbrišejo.</span><span class="sxs-lookup"><span data-stu-id="1704a-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="1704a-106">\*\* Opomba\*\* Za to čiščenje so primerni samo predmeti naprave MDM.</span><span class="sxs-lookup"><span data-stu-id="1704a-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="1704a-107">Izključeni so samo predmeti naprave EAS.</span><span class="sxs-lookup"><span data-stu-id="1704a-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="1704a-108">Za dodatne informacije o tem, kdaj naprava postane primerna za izbris na podlagi nastavitve čiščenja naprave in njenega "stanja":</span><span class="sxs-lookup"><span data-stu-id="1704a-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="1704a-109">Nastavitev: **Brisanje naprav po zadnjem datumu prijave: Da (določena vrednost (N) v določenih dneh)**</span><span class="sxs-lookup"><span data-stu-id="1704a-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="1704a-110">Na podlagi vrednosti (N), konfigurirane v nastavitvi, storitev Intune izbriše napravo v določenih dneh po tem, ko se je nazadnje uspešno všli.</span><span class="sxs-lookup"><span data-stu-id="1704a-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="1704a-111">Nastavitev: **Brisanje naprav po zadnjem datumu prijave: Ne**</span><span class="sxs-lookup"><span data-stu-id="1704a-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="1704a-112">180 dni po izteku veljavnosti potrdila o napravi in se ne obnovi, se naprava izbriše.</span><span class="sxs-lookup"><span data-stu-id="1704a-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="1704a-113">\*\* Opomba\*\* V obeh primerih mora biti naprava uspešno registrirana v intunu.</span><span class="sxs-lookup"><span data-stu-id="1704a-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="1704a-114">Registracija se zgodi med prvim preverjanjem naprave s storitvijo Intune.</span><span class="sxs-lookup"><span data-stu-id="1704a-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="1704a-115">Če se naprava uspešno vpiše v intune, vendar ne registrira intune, se naprava izbriše 270 dni po vpisu.</span><span class="sxs-lookup"><span data-stu-id="1704a-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="1704a-116">(90 dni, da označite napravo kot preklicano, nato pa še 180 dni za brisanje zapisa.)</span><span class="sxs-lookup"><span data-stu-id="1704a-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="1704a-117">Trenutno v konzoli Intune trenutno ni mehanizma za določitev datuma poteka certifikata naprave za katero koli napravo.</span><span class="sxs-lookup"><span data-stu-id="1704a-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>