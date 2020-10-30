---
title: InTune Exchange na mestu uporabe
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808141"
---
# <a name="intune-exchange-on-premise-connector"></a>InTune Exchange na mestu uporabe

Če želite več informacij o nastavitvi povezovalnika med InTune in Exchangeem, ki gostuje na mestu uporabe, si oglejte to dokumentacijo:

[Nastavitev priključka za Exchange na mestu uporabe v programu Microsoft InTune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ**

V: pri poskusu nastavljanja Exchangeevega povezovalnika se prikaže sporočilo o napaki, kot je» različica Exchangeevega povezovalnika ni podprta «. Kaj bi lahko bil vzrok?

A: račun, ki ga uporabljate, je ustrezno licenciran – to mora imeti aktivno licenco za InTune.

V: ali je mogoče imeti več Exchangeevih priključkov?

A: nastavite lahko le en Exchangeev povezovalnik na InTune najemnika na Exchangeevo organizacijo. Povezovalnik je mogoče namestiti le v en strežnik v organizaciji v več strežnikih Exchange.

Prav tako ne morete imeti povezovalnikov, konfiguriranih za Exchange na mestu uporabe in Exchange Online, konfigurirane v istem najemniku.

V: ali lahko povezovalnik uporabi polje CAS za povezavo s storitvijo Exchange?

A: določanje matrike CAS ni podprta konfiguracija v nastavitvi povezovalnika. Navedeni bi moral biti le en strežnik in bi moral biti hardcoded v konfiguracijski datoteki povezovalnika, ki jo je mogoče najti v

program data\microsoft\microsoft InTune na strežniku Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Poiščite ta vnos ```<ExchangeWebServiceURL />``` in zamenjajte spletni naslov z Exchangeevim strežnikom.

**Primer**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Oglejte si to dokumentacijo za dodatno odpravljanje težav: [Odpravljanje težav s povezovalnikom strežnika Exchange na mestu uporabe](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Omogočanje obširnega pisanja dnevnika za Exchangeev povezovalnik**

1. Odprite konfiguracijsko datoteko sledenja priključka za Exchange za urejanje.  
Datoteka se nahaja na spletnem mestu:%ProgramData%\Microsoft\Windows InTune Exchange Connector\TracingConfiguration.xml  

**Primer**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Poiščite TraceSourceLine s tem ključem: OnPremisesExchangeConnectorService  
  
3. Spreminjanje vrednosti vozlišča SourceLevel iz ActivityTracing informacij (privzeto) na verbose ActivityTracing  

**Primer**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Vnovični zagon storitve Microsoft InTune Exchange  
5. Popolna sinhronizacija v portalu InTune, dokler se ne dokonča in nato spremenite XML v» informacije ActivityTracing «in znova zaženite storitev Microsoft InTune Exchange.  
6. Lokacija dnevnikov je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`