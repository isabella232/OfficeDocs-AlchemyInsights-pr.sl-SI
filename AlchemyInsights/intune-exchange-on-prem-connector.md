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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="a3113-102">InTune Exchange na mestu uporabe</span><span class="sxs-lookup"><span data-stu-id="a3113-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="a3113-103">Če želite več informacij o nastavitvi povezovalnika med InTune in Exchangeem, ki gostuje na mestu uporabe, si oglejte to dokumentacijo:</span><span class="sxs-lookup"><span data-stu-id="a3113-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="a3113-104">Nastavitev priključka za Exchange na mestu uporabe v programu Microsoft InTune Azure</span><span class="sxs-lookup"><span data-stu-id="a3113-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="a3113-105">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="a3113-105">**FAQ:**</span></span>

<span data-ttu-id="a3113-106">V: pri poskusu nastavljanja Exchangeevega povezovalnika se prikaže sporočilo o napaki, kot je» različica Exchangeevega povezovalnika ni podprta «.</span><span class="sxs-lookup"><span data-stu-id="a3113-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="a3113-107">Kaj bi lahko bil vzrok?</span><span class="sxs-lookup"><span data-stu-id="a3113-107">What could be the cause?</span></span>

<span data-ttu-id="a3113-108">A: račun, ki ga uporabljate, je ustrezno licenciran – to mora imeti aktivno licenco za InTune.</span><span class="sxs-lookup"><span data-stu-id="a3113-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="a3113-109">V: ali je mogoče imeti več Exchangeevih priključkov?</span><span class="sxs-lookup"><span data-stu-id="a3113-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="a3113-110">A: nastavite lahko le en Exchangeev povezovalnik na InTune najemnika na Exchangeevo organizacijo.</span><span class="sxs-lookup"><span data-stu-id="a3113-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="a3113-111">Povezovalnik je mogoče namestiti le v en strežnik v organizaciji v več strežnikih Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3113-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="a3113-112">Prav tako ne morete imeti povezovalnikov, konfiguriranih za Exchange na mestu uporabe in Exchange Online, konfigurirane v istem najemniku.</span><span class="sxs-lookup"><span data-stu-id="a3113-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="a3113-113">V: ali lahko povezovalnik uporabi polje CAS za povezavo s storitvijo Exchange?</span><span class="sxs-lookup"><span data-stu-id="a3113-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="a3113-114">A: določanje matrike CAS ni podprta konfiguracija v nastavitvi povezovalnika.</span><span class="sxs-lookup"><span data-stu-id="a3113-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="a3113-115">Navedeni bi moral biti le en strežnik in bi moral biti hardcoded v konfiguracijski datoteki povezovalnika, ki jo je mogoče najti v</span><span class="sxs-lookup"><span data-stu-id="a3113-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="a3113-116">program data\microsoft\microsoft InTune na strežniku Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="a3113-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="a3113-117">Poiščite ta vnos ```<ExchangeWebServiceURL />``` in zamenjajte spletni naslov z Exchangeevim strežnikom.</span><span class="sxs-lookup"><span data-stu-id="a3113-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="a3113-118">**Primer**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="a3113-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="a3113-119">Oglejte si to dokumentacijo za dodatno odpravljanje težav: [Odpravljanje težav s povezovalnikom strežnika Exchange na mestu uporabe](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="a3113-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="a3113-120">**Omogočanje obširnega pisanja dnevnika za Exchangeev povezovalnik**</span><span class="sxs-lookup"><span data-stu-id="a3113-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="a3113-121">Odprite konfiguracijsko datoteko sledenja priključka za Exchange za urejanje.</span><span class="sxs-lookup"><span data-stu-id="a3113-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="a3113-122">Datoteka se nahaja na spletnem mestu:%ProgramData%\Microsoft\Windows InTune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="a3113-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="a3113-123">**Primer**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="a3113-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="a3113-124">Poiščite TraceSourceLine s tem ključem: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="a3113-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="a3113-125">Spreminjanje vrednosti vozlišča SourceLevel iz ActivityTracing informacij (privzeto) na verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="a3113-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="a3113-126">**Primer**</span><span class="sxs-lookup"><span data-stu-id="a3113-126">**Example:**</span></span>
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
4. <span data-ttu-id="a3113-127">Vnovični zagon storitve Microsoft InTune Exchange</span><span class="sxs-lookup"><span data-stu-id="a3113-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="a3113-128">Popolna sinhronizacija v portalu InTune, dokler se ne dokonča in nato spremenite XML v» informacije ActivityTracing «in znova zaženite storitev Microsoft InTune Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3113-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="a3113-129">Lokacija dnevnikov je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="a3113-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>