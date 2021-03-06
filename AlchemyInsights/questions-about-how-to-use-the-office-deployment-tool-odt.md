---
title: Domande su come usare lo Strumento di distribuzione di Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790336"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Domande su come usare lo Strumento di distribuzione di Office (ODT)

Scaricare lo Strumento di distribuzione di Office dall'[Area download Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Dopo il download del file, eseguire il file eseguibile autoestraente, che contiene il file eseguibile dello Strumento di distribuzione di Office (setup.exe) e un file di configurazione di esempio (configuration.xml).
  
 **Per escludere o rimuovere i prodotti Microsoft 365 Apps for enterprise dai computer client:**
  
Quando si installa Microsoft 365 Apps for enterprise, è possibile escludere prodotti specifici. A questo scopo, seguire i passaggi per installare Office con lo strumento ODT, ma includere l'elemento ExcludeApp nel file di configurazione. Ad esempio, questo file di configurazione installa tutti i prodotti Microsoft 365 Apps for enterprise ad eccezione di Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Panoramica dello Strumento di distribuzione di Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

