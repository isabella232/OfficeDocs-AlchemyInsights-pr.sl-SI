---
title: Zakaj je gumb» Dodaj predračun «onemogočen zame?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807670"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Zakaj je gumb» Dodaj predračun «onemogočen zame?

Če želite ustvariti predračun, potrebujete eno od teh dovoljenj:

- Skupina» upravljanje «,» naročnina «, obsegi skupine virov
- Sodelavec za upravljanje stroškov
- Lastnik
- Sodelavec
- Le odjemalec podjetja: vpis, oddelek, obsegi računa
- Skrbnik za vpis (nastavitev proračuna na obseg vpisa)
- Skrbnik oddelka (nastavitev proračuna na področju uporabe oddelka)
- Lastnik računa (nastavitev proračuna na obseg računa)
- Sodobni sporazum stranke: račun za obračunavanje, profil obračunavanja, obsegi razdelka z računom
- Naročnina na Azure

**Ustvaril sem predračun, ko je bil moj strošek za trenutni mesec že presežen predračun. Zakaj nisem prejel opozorila?**  
Če ste že presegli določen prag stroška, ko ustvarite predračun, ki ga opozorilo ne bo zažgalo. Ko se začne nov cikel, če prekoračite prag, se bo opozorilo zažgalo.

**Kdaj naj pričakujem, da prejmem opozorilo, ko presežem eno od mojih določenih pragov predračunskih opozoril?**  
Proračuni so ovrednoteni vsake 4 ure. Če želite doseči sistem proračunov, traja najmanj 8 ur za uporabo podatkov. Zaradi tega lahko opozorila trajajo največ 12 ur, ko presežete prag.

**Zakaj je gumb» začetni datum «onemogočen, ko izberem mesec ali obdobje ponastavljanja meseca za obračun?**  
Proračuni so poravnani s trenutnim koledarjem ali trenutnim obdobjem obračunavanja (v primeru, ko je izbran mesečni obračun). Zato smo vnaprej zapolnili to vrednost za vas.

**Zakaj ne vidim grafa mojih stroškov v izkušnji ustvarjanja proračuna?**  
Potrebujemo vsaj 2 meseca podatkov o stroških, preden lahko naredimo graf, ki vam bo pomagal pri ustvarjanju proračuna.

**Zakaj ne morem nastaviti predračuna za naročnino, ki sem jo pravkar ustvaril?**  
Po nastanku naročnine podatki trajajo 24-48 ur, preden nastavite predračun.

**Viri sredstev API**

- [Proračuni API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): zagotavlja operacije za ustvarjanje in posodabljanje proračunov. Z API-ji predračunov lahko nastavite prag predračuna in nastavite več opozoril na ogenj, ko se približate temu pragu. Opozorila lahko sprožijo e-poštno ali Azure skupino dejanj za izvajanje avtomatizacije. Opomba: filtriranje za ta API se ne poravna s filtriranjem in dimenzijami API poizvedbe.
- [Proračuni API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): ustvarjanje proračunov z večjimi možnostmi filtriranja stroškov kot v1. Filtriranje poravna s pogodbo, ki se uporablja v naših poizvedbah in dimenzijah API-ji. To je priporočena proračunska API za uporabo premikanja naprej.
- [Dimenzije](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): zagotavlja postopke za pridobivanje podprtih dimenzij za vašo uporabo v okviru različnih obsegov. Z dimenzijami API lahko pridobite seznam dimenzij, ki jih lahko uporabite kot vložke za generiranje poizvedb s poizvedbo API.
- [Poizvedba](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): zagotavlja operacije, če želite dobiti Združene stroške in podatke o uporabi, ki temeljijo na poizvedbi, ki jo dobavljate. Z uporabo API-ja poizvedbe lahko določite želeno filtriranje, razvrščanje in združevanje na vseh razpoložljivih dimenzijah (do katerih dostopate v API-jih dimenzij).

**Predvideni stroški**

**Zakaj ne vidim napovedi za svoje stroške v analizi stroškov?**  
Obstaja več razlogov, zakaj je projekcija napovedi morda pogrešana za vas v razdelku analiza stroškov, nekateri od njih so naslednji:

1. Če so podatki o stroških mlajši od 10 dni, grafikon napovedi ne bo obremenjen. Model zahteva vsaj 10 dni nedavnih podatkov o stroških za natančne projekcije.
2. Če ste izbrali zgodovinske datume, grafikon» napoved «ne bo viden. Izberite datumski obseg s prihodnjimi datumi za prikaz grafikona napovedi.
3. Če je v vašem računu več valut, bo grafikon napovedi predstavljal le stroške projekta za» vse stroške v USD «.

**Zakaj se napoved ne spremeni, ko spremenim svoje vire?**  
Model predvidevanja zahteva nekaj dni, da upošteva spremembe v računu in ne izvede takojšnjih projekcij na podlagi sprememb virov  
Če želite večje korake povečanja ali zmanjšanja virov, bo model trajal nekoliko dlje, da se bodo te spremembe prilagodile spremembam za nepravilnosti.

**Zakaj se moja napoved poveča, ko rezerviram rezervacijo ali nakup tržnice?**  
Model predvidevanja upošteva vaše» dejanske stroške «in ne upošteva uporabe in nakupa posebej. Za enkratni nakup bo model znižal projekcije po 10 dneh, da upošteva nenadno povečanje stroškov.

**Želim si ogledati napovedi za eno dimenzijo (npr. Meter**  
Napoved trenutno podpira skupne projekcije stroškov in ne za posamezne števce. Ko je argument» združen z «dimenzije, bodo projekcije za skupno vsoto vseh elementov v dimenziji.

**Priporočeni dokumenti**

- [Kaj je upravljanje stroškov Azure?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najboljše prakse za upravljanje stroškov Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizirajte stroške in porabo](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Raziskovanje in analiza stroškov z analizo stroškov](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Upravljanje stroškov Azure: oblikovanje cen](https://azure.microsoft.com/services/cost-management/#pricing)
- [Pregled stroškov v analizi stroškov](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Vadnica za videoposnetke: ustvarjanje proračuna v portalu Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Zahteve za ogled in prilagajanje proračunov](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Ustvarjanje in upravljanje proračunov](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfiguracija avtomatizacije z akcijskimi skupinami Azure in predračuni API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Uporaba opozoril o stroških za nadzorovanje uporabe in porabe](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najboljše prakse za upravljanje stroškov](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Vadnica za videoposnetke**

- [Ustvarjanje proračuna v portalu Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Upravljanje stroškov s Podračuni API in akcijske skupine](https://go.microsoft.com/fwlink/?linkid=2147038)