---
title: Risolvere l'errore L'applicazione non è stata rilevata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810488"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Risolvere l'errore "L'applicazione non è stata rilevata"

L'errore di installazione dell'app "L'applicazione non è stata rilevata dopo il completamento dell'installazione" segnalato da Intune potrebbe comparire in tutte le principali piattaforme di sistemi operativi (Windows, iOS e Android).

Gli scenari più comuni che generano questo errore includono:

- L'app è stata aggiornata all'esterno di Intune (da un App Store di terze parti) dopo la distribuzione iniziale. Ad esempio, alcune applicazioni come Google Chrome potrebbero eseguire gli aggiornamenti automatici.
- Dopo l'installazione iniziale, un utente ha disinstallato l'app.

Per ovviare a questo problema, eseguire prima di tutto una revisione dei dispositivi interessati per determinare lo scenario in cui si verifica l'errore.

- Se l'app è stata aggiornata all'esterno di Intune, la distribuzione dell'app potrebbe essere stata impostata per ignorare la versione dell'applicazione. A questo scopo, in **Configurazione dell'app > Informazioni sull'app** impostare **Ignora la versione dell'app** su **Sì**.
- Durante l'assegnazione del client, potrebbe essere opportuno distribuire l'applicazione come "obbligatoria" e assicurarsi che venga distribuita l'ultima versione.
- In alternativa, nella piattaforma iOS è possibile usare la funzionalità di **aggiornamento automatico** associata al Volume Purchase Program di Apple, che può essere configurata per l'aggiornamento automatico alle nuove versioni di applicazioni quando diventano disponibili.

Per altre informazioni sulla risoluzione dei problemi di installazione delle app, vedere [Risoluzione dei problemi di installazione delle app](https://docs.microsoft.com/intune/troubleshoot-app-install).