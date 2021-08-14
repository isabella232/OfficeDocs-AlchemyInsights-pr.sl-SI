---
title: Napake v aplikaciji
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931465"
---
# <a name="application-errors"></a>Napake v aplikaciji

Iščete informacije o kodah napak **AADSTS,** ki jih vrne storitev varnostnega žetona Azure Active Directory (Azure AD) (STS)? Preberite [kode napak preverjanja pristnosti imenika Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) in kode napak s pooblastilom, da najdete opise napak, popravke in nekatere predlagane rešitve za AADSTS.

Vzrok za napake avtorizacije so lahko različne težave – večina težav javi napako 401 ali 403. Na primer, vse to lahko povzroči napake pri avtorizacijah:

- Napačni [poteki pridobivanja žetona za dostop](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Neustrezno konfigurirani [obsegi dovoljenja](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Manjkajoče [soglasje](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Če želite odpraviti pogoste napake s pooblastilom, poskusite odpraviti napake, ki so navedene spodaj in se najbolj ujemajo z napako, ki ste jo prejeli. Morda je zahtevanih več.

**Napaka »401 Nepooblaščeno«: Ali je vaš žeton veljaven?**

Prepričajte se, da vaša aplikacija predstavlja veljaven žeton za dostop za Microsoft Graph kot del zahteve. Ta napaka običajno pomeni, da v glavi zahteve za preverjanje pristnosti HTTP manjka žeton za dostop ali pa žeton ni veljaven oziroma je potekel. Toplo priporočamo, da uporabite Microsoftovo knjižnico preverjanja [pristnosti (MSAL) za](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) pridobivanje žetonov za dostop. Do te napake lahko pride tudi, če poskušate uporabiti žeton za pooblaščeni dostop, dodeljen osebnemu Microsoftovemu računu, za dostop do API-ja, ki podpira le službene ali šolske račune (račun organizacije).

**Napaka »403 Prepovedano«: Ali ste izbrali ustrezen nabor dovoljenj?**

Preverite, ali ste zahtevali pravilen nabor dovoljenj, ki temeljijo na vmesnikih API Graph Microsoft Graph klici v aplikaciji. Priporočena dovoljenja z najmanj prednostmi so na voljo v vseh temah za referenčno metodo GRAPH Microsoft Graph API. Ta dovoljenja mora za aplikacijo odobriti uporabnika ali skrbnik. Dodeljevanje dovoljenj po navadi se dogaja na strani za soglasje ali tako, da odobrite dovoljenja z orodjem za registracijo aplikacije Azure Portal. Na listu **Nastavitve** za aplikacijo kliknite **Zahtevana dovoljenja**, nato pa kliknite **Odobri dovoljenja**.

- [Dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumevanje dovoljenj in soglasja za Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Napaka »403 Prepovedano«: Ali je aplikacija pridobila žeton, ki ustreza izbranim dovoljenjem?**

Prepričajte se, da se vrsta zahtevanih ali podeljenih dovoljenj ujema z vrsto žetona za dostop, ki ga pridobi program. Morda zahtevate in podeljujete dovoljenja za aplikacijo, vendar namesto žetonov poteka odjemalskih poverilnic uporabljate pooblaščene interaktivne kode ali pa zahtevate in dodelite pooblaščena dovoljenja, vendar namesto žetonov poteka kode uporabite žetone za odjemalce s poverilnicami toka.

- [Pridobivanje dostopa v imenu uporabnikov in pooblaščenih dovoljenj](https://docs.microsoft.com/graph/auth_v2_user) 
- [Tok avtorizacijske kode Azure AD v2.0 - OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Pridobivanje dostopa brez uporabnika (storitev strežniškega procesa) in dovoljenj za aplikacijo](https://docs.microsoft.com/graph/auth_v2_service) 
- [Tok poverilnic odjemalca Azure AD v2.0 - OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Napaka »403 Prepovedano«: ponastavitev gesla**

Trenutno ni nobenega strežniškega procesa za dovoljenja »od storitve do storitve« za aplikacijo, ki omogočajo ponastavitev gesel. Ti vmesniki API so podprti le za uporabo tokov interaktivne pooblaščene kode z vpisanim skrbnikom.

- [Dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**»403 Prepovedano«: Ali ima uporabnik dostop in ustrezno licenco?**

Za poteke pooblaščene kode Microsoft Graph oceni, ali je zahteva dovoljena glede na dovoljenja, dodeljena aplikaciji, in dovoljenja, ki jih ima vpisani uporabnik. Ta napaka običajno označuje, da uporabnik nima prednostnih dovoljenj za izvajanje zahteve ali pa nima licence za dostop do podatkov. Zahtevo lahko uspešno izvedejo le uporabniki z zahtevanimi dovoljenji ali licencami.

**»403 Prepovedano«: Ali ste izbrali pravilen vmesnik API vira?**

Storitve API, kot je Microsoft Graph preverite, ali se zvočni zahteva (občinstvo) v žetonu za prejet dostop ujema z vrednostjo, ki jo pričakuje sama, in če ni, se prikaže sporočilo o napaki »403 – prepovedano«. Običajno do te napake pride, ker poskušate uporabiti žeton, pridobljen za vmesnike API za Azure AD Graph, vmesnike API za Outlook ali vmesnike API za SharePoint/OneDrive, da bi priklicali Microsoft Graph (ali obratno). Zagotovite da se vir (ali obseg), za katerega aplikacija želi pridobiti žeton, ujema z vmesnikom API, ki ga aplikacija želi priklicati.

**»400 Neprimerna zahteva« ali »403 Prepovedano«: Ali uporabnik deluje v skladu s pravilnikom o pogojnem dostopu organizacije?**

Glede na pravilnike cajta organizacije je uporabnik, ki dostopa do virov storitve Microsoft Graph prek vaše aplikacije, morda zahteva dodatne informacije, ki jih ni v žetonu za dostop, ki ga je prvotno pridobil program. V tem primeru je v aplikaciji javljena napaka 400 *zahtevana_interakcija* med pridobivanjem žetona za dostop ali pa napaka 403 *nezadostne_zahteve* med izvajanjem postopka klicanja vmesnika Microsoft Graph. V obeh primerih odgovor o napaki vsebuje dodatne informacije, ki jih je mogoče predstaviti pooblaščeni končni točki za izziv uporabnika z dodatnimi informacijami (kot je večkratno preverjanje pristnosti ali včlanitev naprave).

- [Upravljanje izziva s pogojnim dostopom s storitvijo MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Navodila za razvijalce za pogojni dostop za Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
