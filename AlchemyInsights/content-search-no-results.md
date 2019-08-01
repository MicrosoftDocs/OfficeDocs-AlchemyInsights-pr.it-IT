---
title: Ricerca contenuto nessun risultato
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800426"
---
# <a name="no-results-from-content-searchexports"></a>Nessun risultato dalla ricerca contenuto/esportazioni

Problemi relativi alla ricerca di contenuto/esportazioni la mancata restituzione di dati potrebbe essere dovuta a un determinato filtro di sicurezza di conformità che è stato configurato da un amministratore specifico e che non lo ha comunicato a tutti gli amministratori.

Per risolvere il problema, verificare se sono presenti filtri di sicurezza per la conformità che potrebbero causare questo problema:
1. Connettersi a PowerShell per Centro sicurezza e conformità
2. Eseguire le seguenti commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org