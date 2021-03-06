---
title: Microsoft teams-accesso Guest
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: ee38dcb5f40ea16cea1b84b9b16e86b0f52f2d89
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/13/2020
ms.locfileid: "48452232"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft teams-accesso Guest

Se si ha bisogno di assistenza per la comunicazione con gli utenti esterni all'organizzazione in team, è necessario decidere se utilizzare [l'accesso guest o l'accesso esterno (Federazione)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)oppure è possibile utilizzarli entrambi.

Assicurarsi di [esaminare le differenze](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) per comprendere le funzionalità disponibili per ogni.  Ad esempio, l'accesso esterno (Federation) consente comunicazioni di 1:1, come chat e presenza.  Gli utenti federati non possono partecipare alla collaborazione di teams tuttavia.  Se si desidera che un utente esterno partecipi a conversazioni di canale di team o di condivisione di file, è necessario abilitare l'accesso guest.

**Opzione 1: abilitare l'accesso Guest** Nell'interfaccia di amministrazione di teams, accedere a [impostazioni di org Wide > Guest Access](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) e attivare "Consenti accesso guest in teams".  Per un tenant con tutte le altre impostazioni predefinite, questo dovrebbe essere tutto quello che devi fare.  Per personalizzare la configurazione dell'accesso guest, accertarsi di seguire tutti i passaggi riportati nell' [elenco di controllo di accesso Guest](https://docs.microsoft.com/microsoftteams/guest-access-checklist). Una volta completata l'operazione, sarà necessario [attendere fino a 24 ore](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) per rendere effettive le impostazioni.

Se si è certi di aver completato tutti i passaggi dell'elenco di controllo e sono passate più di 24 ore, provare a [aggiungere un ospite al team](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).

Per ulteriori informazioni, inclusi i video su come fare, vedere [Guest Access in Microsoft teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Opzione 2: attiva accesso esterno (Federazione)** Se si desidera anche abilitare l'accesso esterno (Federazione), nell'interfaccia di amministrazione del team passare a impostazioni a livello di organizzazione [> accesso esterno](https://admin.teams.microsoft.com/company-wide-settings/external-communications) e attiva "gli utenti possono comunicare con Skype for Business and Teams Users" e quindi seguire tutti i passaggi descritti in [Let your teams gli utenti chattare e comunicare con gli utenti in un'altra organizzazione](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).
