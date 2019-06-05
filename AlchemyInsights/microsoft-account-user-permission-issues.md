---
title: Ustvarite in uporabljate nabiralnik v skupni rabi
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717362"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Odpravljanje težave - uporabnika ni mogoče najti v imeniku

<p>Če uporabniki se prikazuje sporočilo o napaki <strong> &ldquo; &hellip;uporabnik lahko&rsquo;t je mogoče najti v imeniku. Poskusite znova&hellip; </strong> kjer vrsto izdaje je <strong> &ldquo;uporabnik ni v imeniku.&rdquo;</strong>, odpraviti težavo mogoče dokončati naslednje korake.</p> <ol> <li>Zagotovitev račun, ki je sprejel povabilo email je isti račun, ki se uporablja za vpis v kasneje. Preverite, ali uporabnik uporablja isti račun sprejmite povabilo, in sicer v mestu. <br /><br />Za več informacij, glejte <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">kako upravljati vzdevki za račun Microsoft</a> za upravljanje prijavo Office 365. <br /><br /></li> <li>Prebrskajte do vsakega območja(-ij), v katerem uporabnik prejema napako. <br /><br />a. Dodaj <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (znotraj dvojnih narekovajev) v prenehati od URL mesta. <br /><br />Primer: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Na seznamu izberite uporabnika. <br /><br />c. Kliknite <strong>Odstrani uporabniška dovoljenja na traku</strong>. <br /><br />d. Dodajte nazaj uporabnika in znova pošljite prositi da uporabnik.</li> </ol>

