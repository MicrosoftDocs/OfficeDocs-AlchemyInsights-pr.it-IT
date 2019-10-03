---
title: Impostazioni di criteri per le riunioni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376700"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gestire i criteri di riunione in Microsoft Teams

I criteri di riunione vengono utilizzati per controllare le funzionalità disponibili per i partecipanti alla riunione per le riunioni pianificate dagli utenti dell'organizzazione. Alcune funzionalità dei criteri di riunione potrebbero non essere implementate nell'interfaccia di amministrazione di Teams (queste sono etichettate come "prossimamente" nella documentazione). In questo caso, o se si riceve un errore come "non è possibile aggiornare il criterio in questo momento, ma riprovare più tardi" nell'interfaccia di amministrazione di Microsoft teams, si consiglia di utilizzare PowerShell per creare o modificare i criteri di riunione dei team. 

Per ulteriori informazioni sui criteri di riunione, vedere le risorse seguenti:

- Per ulteriori informazioni sulla creazione di criteri, la modifica e l'assegnazione degli utenti ai criteri, vedere [Manage meeting Policies in teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Per apportare modifiche ai criteri utilizzando i cmdlet di PowerShell, vedere [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - È necessario utilizzare il [modulo di PowerShell di Skype for business](https://www.microsoft.com/download/details.aspx?id=39366) per i criteri di riunione dei team. 
    - Per ulteriori informazioni, vedere la [documentazione relativa ai cmdlet *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .

**Nota:** Per rendere effettive le modifiche ai criteri per gli utenti, è possibile richiedere fino a 24 ore. Potrebbe non essere possibile apportare modifiche ai criteri appena creati immediatamente. attendere 4 ore e tentare di modificare nuovamente un criterio appena creato. Se si verificano ancora problemi, provare PowerShell.  