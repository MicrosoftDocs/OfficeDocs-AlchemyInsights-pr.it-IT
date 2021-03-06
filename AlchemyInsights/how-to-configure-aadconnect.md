---
title: 646 come configurare AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704493"
---
# <a name="configure-sync-features"></a>Configurare le funzionalità di sincronizzazione

Azure AD Connect include diverse funzionalità che sono abilitate per impostazione predefinita o che possono essere abilitate in un secondo momento. Alcune funzionalità richiedono una configurazione aggiuntiva in ambienti specifici.

- Limiti del [filtro](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) gli oggetti vengono sincronizzati con Azure ad. Per impostazione predefinita, tutti gli utenti, i contatti, i gruppi e gli account computer di Windows 10 sono sincronizzati. È possibile includere o escludere oggetti basati su domini, unità organizzative o altri attributi.

- [Sincronizzazione hash password](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincronizza l'hash della password da Active Directory locale AD Azure ad. In questo modo la gestione delle password viene consentita in una posizione, ma viene utilizzata la stessa password sia in ambienti locali che in quelli cloud. Poiché Active Directory è l'origine autorevole, è possibile utilizzare i criteri di password personalizzati.

- La [reimpostazione della password in modalità self-service (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) consente agli utenti di reimpostare le proprie password nel cloud pur applicando i criteri di password locali.

- Il [writeback del dispositivo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) consente ai dispositivi registrati in Azure ad di essere riscritti in Active Directory locale in modo che possano essere utilizzati per l'accesso condizionale.

- [Impedisci eliminazioni accidentali](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) è abilitata per impostazione predefinita per evitare troppe eliminazioni simultanee degli oggetti (più di 500 Object per sincronizzazione). È possibile modificare questa impostazione in modo da soddisfare le esigenze dell'organizzazione.

- L' [aggiornamento automatico](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) è abilitato per impostazione predefinita per le installazioni Express e garantisce che la versione di Azure ad Connect sia sempre aggiornata.
