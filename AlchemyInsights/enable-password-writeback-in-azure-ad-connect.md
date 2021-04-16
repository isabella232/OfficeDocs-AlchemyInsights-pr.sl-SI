---
title: Omogočanje gesla writeback v storitvi Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814028"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Omogočanje gesla writeback v storitvi Azure AD Connect

Če želite omogočiti samopostrežno ponastavitev gesla writeback, najprej omogočite možnost writeback v storitvi Azure AD Connect. Iz strežnika Azure AD Connect Server dokončajte te korake:

1. Vpišite se v strežnik Azure AD Connect Server in zaženite čarovnika za konfiguracijo **Azure AD Connect**.
2. Na **pozdravni** strani kliknite **Naprej**. 
3. Na strani **dodatna opravila** izberite **prilagodite možnosti sinhronizacije** in nato kliknite **naprej**.
4. V **Povežite se s stranjo Azure AD**, vnesite poverilnico globalnega skrbnika za svojega najemnika Azure in nato kliknite **naslednja**.
5. V **povežite imenike** in **Domain/OU** filtrirajte strani, kliknite **naprej**.
6. Na strani **izbirne funkcije** potrdite polje ob možnosti **geslo writeback** in kliknite **naprej**.
7. Na strani **pripravljena** konfigurirati tako, da kliknete **Konfiguriraj** in počakate, da se postopek dokonča.
8. Ko vidite konfiguracijo Dokončaj, kliknite **Exit**.

Z geslom writeback omogočeno v storitvi Azure AD Connect, konfigurirajte Azure AD SSPR za writeback.  Če želite omogočiti geslo writeback v SSPR, dokončajte te korake:

1. Vpišite se v portal Azure z uporabo globalnega skrbniškega računa.
2. Poiščete in izberete **imenika Azure Active Directory**, kliknite **ponastavitev gesla**, nato pa kliknite **integracija na mestu uporabe**.
3. Nastavitev možnosti za **geslo za pisanje nazaj v imenik na mestu uporabe?** za **da**.
4. Nastavitev možnosti za **dovoli uporabnikom, da odklenejo račune, ne da bi morali ponastaviti svoje geslo?** za **da**.
5. Ko končate, kliknite **Dokončano**.

Če želite več informacij, glejte [omogočite samopostrežno ponastavitev gesla imenika Azure Active Directory, ki je na voljo v okolju na mestu uporabe,](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)writeback.

> [!NOTE]
>  Ko skrbnik Ponastavi geslo uporabnika v portalu Azure, če je ta uporabnik povezan ali da je Razpršilo z geslom sinhronizirano, je geslo znova zapisano na mestu uporabe. Za to funkcijo potrebujete licenco za Azure Premium (P1 ali P2) in trenutno ni podprta na Skrbniškem portalu za Office.
