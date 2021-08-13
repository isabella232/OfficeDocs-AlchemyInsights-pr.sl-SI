---
title: Zakaj je gumb za dodajanje proračuna onemogočen?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954696"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Zakaj je gumb za dodajanje proračuna onemogočen?

Če želite ustvariti proračun, potrebujete eno od teh dovoljenj:

- Management Group, Subscription, Resource Group Scopes
- Sodelavec za upravljanje stroškov
- Lastnik
- Sodelavec
- Samo stranka podjetja: včlanitev, oddelek, obsegi računa
- Skrbnik za včlanitev (nastavite proračun na obseg včlanitve)
- Skrbnik oddelka (nastavi proračun na obseg oddelka)
- Lastnik računa (nastavite proračun na obseg računa)
- Samo sodobna pogodba za stranke: račun za obračunavanje, profil za obračunavanje, obsegi razdelka računa
- Avtor naročnine na Azure

**Ustvaril sem proračun, ko so bili moji stroški za trenutni mesec že nad proračunom. Zakaj nisem prejel opozorila?**  
Če ste že presegli določen prag stroškov, ko ustvarite proračun, ki opozorilo ne bo požarno. Ko se začne nov cikel in če kršite prag, se bo opozorilo zaganjali.

**Kdaj naj pričakujem, da bom prejel opozorilo, ko presežem enega od določenih pragov opozoril za proračun?**  
Proračune se ovrednotijo vsakih 4 ure. Podatki o uporabi so v sistemu proračunov dosegljivi v vsaj 8 urah. Glede na to lahko traja do 12 ur, da se opozorila požarijo, ko presežete prag.

**Zakaj je gumb »Začetni datum« onemogočen, ko izberem obdobje ponastavitve meseca ali meseca obračunavanja?**  
Proračuni so poravnani s trenutnim koledarskem mesecem ali trenutnim obdobjem obračunavanja (v primeru, ko je izbrana možnost Mesec obračunavanja). Zato to vrednost vnaprej zapolnimo za vas.

**Zakaj ne vidim grafa mojih stroškov v izkušnji ustvarjanja proračuna?**  
Preden lahko upodobiti graf, ki vam bo pomagal pri ustvarjanju proračuna, potrebujemo najmanj 2 meseca podatkov o stroških.

**Zakaj ne morem nastaviti proračuna za naročnino, ki sem jo pravkar ustvaril?**  
Po tem, ko je bila ustvarjena naročnina, so podatki obdelani v 24–48 urah, preden se proračun ne uporabi.

**Budget API Resources**

- [API proračunov v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Zagotavlja postopke za ustvarjanje in posodabljanje proračunov. Z api-jem za proračune lahko nastavite prag proračuna in konfigurirate več opozoril za požar, ko se boste približali tem pragu. Opozorila lahko sprožijo avtomatizacijo e-pošte ali skupine dejanj Azure. Opomba: Filtriranje za ta API ni poravnano s filtriranjem/dimenzijami API-ja poizvedbe.
- [API proračunov v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)ustvarite proračune z več zmogljivostmi filtriranja stroškov kot v1. Filtriranje se poravna s pogodbo, ki je uporabljena v API-jih za poizvedbo in dimenzije. To je priporočeni API proračunov za uporabo prehoda.
- [Dimenzije:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Ponuja postopke, s katerimi pridobite podprte dimenzije za vašo uporabo v različnih obsegih. Z vmesnikom API dimenzij lahko pridobite seznam dimenzij, ki jih lahko uporabite kot vnose za ustvarjanje poizvedb z API-jem poizvedbe.
- [Poizvedba:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Ponuja postopke za zbiranje podatkov o stroških in uporabi na podlagi poizvedbe, ki jo v dobili. Z api-jem poizvedbe lahko določite želene možnosti filtriranja, razvrščanja in razvrščanja v skupinah za vse razpoložljive dimenzije (do katerih dostopate v API-jih Dimenzije).

**Napovedani stroški**

**Zakaj ne vidim napovedi stroškov v analizi stroškov?**  
Obstaja več razlogov, zakaj napoved morda ne bo na voljo v analizi stroškov, drugi pa so:

1. Če so podatki o stroških stari manj kot 10 dni, se grafikon napovedi ne bo naložil. Model zahteva vsaj 10 dni nedavnih podatkov o stroških za natančne projekcije
2. Če ste izbrali zgodovinska datuma, grafikon napovedi ne bo viden. Izberite datumski obseg s prihodnjimi datumi, da bo grafikon napovedi prikazan
3. Če imate v vašem računu več valut, bodo na grafikonu napovedi le stroški projekta »Vsi stroški v USD«

**Zakaj se napoved ne spremeni, ko spremenim svoje vire?**  
Model napovedi zahteva nekaj dni, da upošteva spremembe v računu in ne naredi takojšnjih projekcij, ki temeljijo na spremembah virov  
Pri večjih korakih za povečanje ali zmanjšanje virov bo model nekoliko dlje časa traja, da se ta sprememba prilagodi zaradi nenavadnih sprememb

**Zakaj se moja napoved poveča po rezervaciji ali nakupu na Tržnici?**  
V modelu napovedi so upoštevani dejanski stroški in ne upošteva uporabe in nakupa ločeno. Pri enkratnem nakupu bo model zmanjšal projekcije po 10 dneh, da bi se stroški zaradi tega najhi še povečali.

**Želim videti napovedi za eno dimenzijo (npr. Meter)**  
Predvidevanje trenutno podpira projekcije skupnih stroškov in ne za posamezne metre. Torej, ko dimenzijo »Združi po« projekcije skupaj za vse elemente v dimenziji

**Priporočeni dokumenti**

- [Kaj je Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najboljše prakse upravljanja stroškov v storitvi Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizirajte stroške in porabo](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Raziskovanje in analiziranje stroškov z analizo stroškov](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Upravljanje stroškov Azure: cene](https://azure.microsoft.com/services/cost-management/#pricing)
- [Pregled stroškov v analizi stroškov](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Videovadnika: ustvarjanje proračuna na portalu Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Zahteve za ogled in prilagajanje proračunov](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Ustvarjanje in upravljanje proračunov](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfiguracija avtomatizacije s skupinami dejanj in API-jem proračunov za Azure](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Uporaba opozoril o stroških za nadzor uporabe in porabe](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najboljše prakse upravljanja stroškov](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Videoposnetki z vadnico**

- [Ustvarjanje proračuna v portalu Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Upravljanje stroškov z API-jem za proračune in skupinami dejanj](https://go.microsoft.com/fwlink/?linkid=2147038)