---
title: Dynamics 365 Forms Business Rules-Business Rule not infornation for a form
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529023"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>L'evento OnChange non si verifica se il campo viene modificato a livello di programmazione

L' ** evento OnChange non si verifica se il campo viene modificato a livello di programmazione tramite l' *attributo.* [](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) SetValue, metodo. Se si desidera che i gestori eventi per ** l'evento OnChange vengano eseguiti dopo aver impostato il valore, è necessario utilizzare l' *attributo formContext. Data. Entity.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) , metodo nel codice.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
