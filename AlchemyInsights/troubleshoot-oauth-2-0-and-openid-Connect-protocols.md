---
title: Odpravljanje težav z OAuth 2,0 in protokoli OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037698"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Odpravljanje težav z OAuth 2,0 in protokoli OpenID Connect

Če želite razrešiti težave s povezovanjem OAuth 2,0 in OpenID, izvedite te priporočene korake:

Oglejte si te članke, ki so povezani s konfiguracijo in odpravljanjem težav z OAuth 2,0 in protokoli OpenID Connect:

- [Platforma Microsoft Identity in OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – v tem članku je opisano, kako program neposredno v skladu s **tokom kode Grant (PKCE)** v aplikaciji, in sicer z uporabo katerega koli jezika.
- [Microsoft Identity platform in tok poverilnic odjemalca OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – v tem članku je opisano, kako program neposredno v primerjavi s **tokom poverilnic odjemalca** v aplikaciji.
- [Poverilnice za gesla za lastnike Microsoft Identity in OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) – v tem članku je opisano, kako program neposredno pred **ROPC tokom** v aplikaciji.
    - Platforma» Microsoftova identiteta «podpira le ROPC za najemnike Azure AD in ne za osebne račune. To pomeni, da morate uporabiti končno točko, določeno za najemnika **( https://login.microsoftonline.com/{TenantId_or_Name})** ali končno točko **organizacije** .
    - Osebni računi, ki so povabljeni v najemnika storitve Azure AD, ne morejo uporabljati ROPC.
    - Računi, ki nimajo gesel, se ne morejo vpisati prek ROPC. Za ta primer priporočamo, da namesto tega uporabite drug tok za svoj program.
    - Če morajo uporabniki uporabiti [multi-Factor Authentication (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) , da se prijavijo v program, bodo blokirani.
    - ROPC ni podprt v scenarijih [hibridne identitete federacije](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (na primer Azure ad in ADFS, ki se uporabljajo za preverjanje pristnosti računov na mestu uporabe). Če so uporabniki v celoti preusmerjeni v ponudnika identitete na mestu uporabe, Azure AD ne more testirati uporabniškega imena in gesla pri ponudniku identitete. [Prepustna preverjanje pristnosti](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) je podprta s ROPC.
    - Izjema v scenariju hibridne identitete je sledeča: pravilnik za odkrivanje domačih sfer z **AllowCloudPasswordValidation** , nastavljeno na **True** , bo omogočil ROPC pretok za delo za Združene uporabnike, ko je geslo na mestu uporabe sinhronizirano z oblakom. Če želite več informacij, glejte [Omogočanje neposrednega preverjanja pristnosti za ROPC za starejše aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Platforma Microsoft Identity in OAuth 2,0 v imenu toka](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) – v tem članku je opisano, kako program neposredno v skladu s **tokom (OBO)** v aplikaciji.
- [Microsoft Identity platform in protokola OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – v tem članku je opisano, kako izvedete protokol za povezavo OpenID neodvisen od jezika in kako pošiljate in PREJEMATE sporočila http brez uporabe Microsoftovih odprtokodnih knjižnic.

**Žetoni za dostop**

[Žetoni za dostop do Microsoftovega](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) uporabniškega vmesnika – Preberite, kako lahko API preveri veljavnost in uporabi terjatve znotraj žetona za dostop. Vsa dokumentacija v tem članku, razen če je označeno, velja le za žetone, izdane za API-je, ki ste jih registrirali. Ne velja za žetone, izdane za Microsoft lastne API-je, ne morete pa uporabiti teh žetonov za preverjanje, kako Microsoftova identitetna platforma izdaja žetone za API, ki jih ustvarite.

**Konfiguracija aplikacije**

[Preusmerjanje uri (odgovor URL) omejitve in omejitve](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – Naučite se konfigurirati uri za preusmeritev (URL odgovora). Preusmeritveni URI ali URL odgovora je mesto, kamor strežnik za avtorizacijo pošlje uporabnika, ko je program uspešno odobril in odobril kodo za avtorizacijo ali žeton za dostop. Strežnik za avtorizacijo pošlje kodo ali žeton v preusmeritveni URI; pomembno je, da registrirate pravilno lokacijo kot del postopka registracije aplikacije.

**Omogočanje uporabe aplikacije**

[Vadnica: priprava in načrtovanje uporabe za SCIM končna točka](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) – v tem članku je opisano, kako ustvarite končno točko SCIM in integrirate s storitvijo za omogočanje uporabe storitve zvočna storitev.


