---
title: Termini mancanti dall'archivio termini di SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750455"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Abilitazione della crittografia BitLocker con Intune

I criteri di protezione dell'endpoint di Intune possono essere utilizzati per configurare le impostazioni di crittografia di Boitlocker per i dispositivi Windows come descritto in: impostazioni di Windows10 (e versioni successive) per proteggere i dispositivi tramite Intune

È necessario tenere presente che molti dispositivi più recenti che eseguono Windows 10 supportano la crittografia automatica di BitLocker che viene attivata senza l'applicazione del criterio MDM. Questo può influire sull'applicazione dei criteri se non sono configurate impostazioni predefinite. Per ulteriori informazioni, vedere FAQ.


Domande frequenti   Q: quali edizioni di Windows supportano la crittografia dei dispositivi utilizzando il criterio di protezione di endpoint?
 A: le impostazioni dei criteri di protezione dell'endpoint di Intune vengono implementate tramite il CSP di BitLocker.Non tutte le edizioni o le build di Windows supportano il CSP di BitLocker. 
      In questo momento le edizioni di Windows: Enterprise; Sono supportate l'istruzione, la telefonia mobile, l'Enterprise Mobile e la Professional (dalla Build 1809 e versioni successive).




D: se un dispositivo è già crittografato con BitLocker utilizzando le impostazioni predefinite del sistema operativo per il metodo di crittografia e la forza di cifratura (XTS-AES-128), l'applicazione di un criterio con impostazioni diverse attiva automaticamente la ricrittografia dell'unità con le nuove impostazioni?

R: No. Per applicare le nuove impostazioni di crittografia, è necessario innanzitutto decrittografare l'unità.

Nota per i dispositivi in fase di registrazione con il pilota automatico la crittografia automatica che si verificherà durante la configurazione guidata non viene attivata fino a quando non viene valutato il criterio di Intune che consente di utilizzare le impostazioni basate sui criteri al posto dei valori predefiniti del sistema operativo.




D se un dispositivo viene crittografato a causa dell'applicazione dei criteri di Intune, la crittografia viene decrittografata quando il criterio viene rimosso?

A: la rimozione dei criteri correlati alla crittografia non comporta la decrittografia delle unità configurate.




D: perché i criteri di conformità di Intune mostrano che il dispositivo non ha "abilitato BitLocker" ma lo è?

A: l'impostazione "BitLocker Enabled" in Intune Compliance Policy utilizza il client di certificazione integrità dispositivo di Windows (DHA). Questo client misura solo lo stato del dispositivo al momento dell'avvio. Pertanto, se un dispositivo non è stato riavviato dopo che è stata completata la crittografia BitLocker, il servizio client DHA non segnalerà BitLocker come attivo.