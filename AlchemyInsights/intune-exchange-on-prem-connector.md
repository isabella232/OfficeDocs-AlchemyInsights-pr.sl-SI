---
title: Intune Exchange na mestu uporabe Connector
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013980"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange na mestu uporabe Connector

Če želite podrobnosti o nastavitvi povezovalnika med intune in Exchange ki gostuje na mestu uporabe, si oglejte to dokumentacijo:

[Nastavitev povezovalnika storitve Intune na mestu Exchange v Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Pogosta vprašanja:**

V: Pri poskusu nastaviti povezovalnik se prikaže napaka, kot je »Različica Exchange Exchange Povezovalnik ni podprta«. Kaj je lahko vzrok?

O: Račun, ki ga uporabljate, je ustrezno licenciran – imeti mora aktivno licenco za Intune.

V: Ali je mogoče imeti več Exchange povezovalnikov?

O: Nastavite lahko le en povezovalnik Exchange na najemnika intune na Exchange organizacije. Povezovalnik je mogoče namestiti le v en strežnik v organizaciji z izmenjavo več strežnikov.

Prav tako ne morete konfigurirati povezovalnikov tako za Exchange na mestu uporabe kot Exchange Online konfigurirani v istem najemniku.

V: Ali lahko povezovalnik uporabi polje CAS kot povezavo do Exchange?

A: Določanje polja CAS ni podprta konfiguracija v nastavitvi povezovalnika. Navesti je treba le en strežnik in ga je treba šidirati v konfiguracijski datoteki povezovalnika, ki jo je mogoče najti v možnosti

program data\microsoft\microsoft Intune na mestu Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Poiščite ta vnos in ```<ExchangeWebServiceURL />``` zamenjajte URL z Exchangeevim strežnikom.

**Primer:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Za dodatno odpravljanje težav si oglejte to dokumentacijo: Odpravljanje težav s priključek storitve [Intune na Exchange mestu uporabe](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Omogočanje pisanja dnevnika »Verbose Exchange povezovalnik**

1. Odprite konfiguracijsko datoteko Exchange sledenje povezovalnika za urejanje.  
Datoteka je na voljo na spletnem mestu: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Primer:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Poiščite TraceSourceLine s tem ključem: OnPremisesExchangeConnectorService  
  
3. Spreminjanje vrednosti vozlišča SourceLevel iz vrednosti Information ActivityTracing (privzeto) v »Verbose ActivityTracing«  

**Primer:**
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
4. Vnovični zagon Microsoft Intune Exchange računalnika  
5. Popolna sinhronizacija v Portalu za Intune, dokler se ne dokonča, nato pa spremenite XML nazaj na »Information ActivityTracing« (Spreminjanje informacij o dejavnosti), nato pa znova zaženite Microsoft Intune Exchange sinhronizacijo.  
6. Mesto dnevnikov je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`