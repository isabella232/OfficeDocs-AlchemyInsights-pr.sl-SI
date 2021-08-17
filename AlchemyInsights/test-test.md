---
title: Manjkajoči pogoji SharePoint spletne shrambe izrazov
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106442"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogočanje šifriranja Bitlocker s funkcijo Intune

S pravilnikom za zaščito končne točke za Intune lahko konfigurirate nastavitve šifriranja Boitlocker za naprave s sistemom Windows, kot je opisano v : Nastavitve sistema Windows10 (in novejše različice) za zaščito naprav z uporabo storitve Intune

Ne pozabite, da številne novejše naprave s sistemom Windows 10 podpirajo samodejno šifriranje bitlocker, ki se sproži brez uporabe pravilnika MDM. To lahko vpliva na uporabo pravilnika, če so konfigurirane nepri privzete nastavitve. Če želite več podrobnosti, glejte Pogosta vprašanja.


Pogosta vprašanja V: Katere izdaje Windows podpirajo šifriranje naprave s pravilnikom za zaščito končne točke?
O: Nastavitve v pravilniku za zaščito končne točke za Intune so posodobljene s programom Bitlocker CSP.  Vse izdaje in Windows ne podpirajo storitve Bitlocker CSP. V tem trenutku Windows izdaje: Enterprise; Podprte so storitve Education, Mobile Enterprise in Professional (od delovne skupine 1809 naprej).




V: Če je naprava že šifrirana s funkcijo Bitlocker s privzetimi nastavitvami operacijskega sistema za način šifriranja in moč cipher (XTS-AES-128), bo pravilnik z različnimi nastavitvami samodejno sprožil ponovno šifriranje pogona z novimi nastavitvami?

O: Ne. Če želite uporabiti nove nastavitve za cipher, morate najprej dešifrirati pogon.

Opomba Za naprave, ki so včlanjene s funkcijo Autopilot, se samodejno šifriranje, ki bi se pojavilo med OOBE, ne sproži, dokler ni ovrednoten pravilnik za Intune, ki omogoča uporabo nastavitev na podlagi pravilnika na mestu privzetih nastavitev operacijskega sistema




V Če je naprava šifrirana zaradi uporabe pravilnika za Intune, ali bo dešifrirana, ko bo ta pravilnik odstranjen?

O: Odstranjevanje pravilnika, povezanega s šifriranjem, NE povzroči dešifriranja pogonov, ki so bili konfigurirani.




V: Zakaj pravilnik o skladnosti storitve intune kaže, da v moji napravi ni omogočena možnost »Bitlocker Enabled«, vendar je?

O: Nastavitev »Bitlocker je omogočena« v pravilniku o skladnosti s predpisi storitve Intune uporablja odjemalca Windows preverjanje ustreznosti stanja naprave (DHA). Ta odjemalec meri le stanje naprave v času zagona. Če torej naprava ni bila znova zagnala, odkar je bilo šifriranje bitlocker dokončano, odjemalska storitev DHA ne prijavi funkcije bitlocker, da je aktivna.