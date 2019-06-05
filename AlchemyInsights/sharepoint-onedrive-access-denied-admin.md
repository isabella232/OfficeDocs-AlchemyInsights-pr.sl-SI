---
title: Odpravljanje težav s postranski tajivec vest
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: ee154a60d80472639371d44faef464eea8734dc9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716662"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Odpravljanje težav s postranski tajivec sporočil v skrbniškem središču za Sharepoint/OneDrive

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Če prejmete sporočilo o zavrnjenem ko poskušate brskati za Sharepoint/OneDrive Admin Center dostopu, prepričajte se, da vam <a href="https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One">dodeli dovoljenje za uporabnika </a>. Če ima uporabnik dovoljenje, prav tako se prepričajte, so <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/about-admin-roles?view=o365-worldwide">dodeljena skrbniška vloga</a> ki lahko dostop do admin centri.</span></p>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Ta težava se lahko pojavi tudi, ko uporabnik izbriše in ponovno ustvari z enakim glavnim imenom uporabnika (UPN). Novi račun je ustvarjen z uporabo različnih PUID (Passport Enolični ID) vrednost. Ko uporabnik poskuša za dostop do zbirke mest ali njihovih OneDrive, uporabnik je napačno PUID. Drugi scenarij vključuje sinhronizacija imenika z Active Directory organizacijska enota (OU). Če uporabniki so že vpisani v SharePoint, in nato preselil v različnih OU in resynced s SharePointom, da lahko pride do te težave.</span></span></p>  <ul style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" type="disc">  <li style="line-height: normal; ; font-size: 11pt; font-style: normal; font-weight: 400;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Če želite težavo odpraviti, obnovite izvirno UPN s korakom v članku, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">obnoviti uporabnik v Office 365</a>.</span></span></li>  </ul>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><strong><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;">Opomba:</span></span></strong><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-fareast-font-family: 'Times New Roman'; mso-bidi-font-family: 'Times New Roman';"><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><em style="mso-bidi-font-style: normal;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;</span></em><em><span style="font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;font-style: normal; mso-bidi-font-style: italic;">Če OneDrive ali SharePoint Admin center ni na voljo za več uporabnikov, ki so prej imeli dostopa, lahko izdajo začasnih storitev.&nbsp; </span></span></em> <em><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;"> <a href="https://portal.office.com/adminportal/home#/servicehealth" target="_blank" rel="noopener"><span style="font-style: normal; mso-bidi-font-style: italic;">Preverite zdravje Nadzorna plošča storitev</span></a>.</span></em></span></span></p>


