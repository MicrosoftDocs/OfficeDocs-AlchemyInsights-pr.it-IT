---
title: Micro ritardi o limitazione in PowerShell per Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702130"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro ritardi o limitazione in PowerShell per Exchange Online

Durante l'esecuzione di script e cmdlet in Exchange Online potrebbero verificarsi ritardi o potrebbero comparire avvisi "Applicato micro ritardo". Seguono alcuni suggerimenti su come risolvere questo problema:

- Eseguire la diagnostica per rivedere i criteri di limitazione di PowerShell del tenant. Nella maggior parte dei casi, questa soluzione risolverà il problema.
- Se il problema non dovesse essersi risolto, provare a usare il [modulo PowerShell per Exchange Online v2](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), che include CMDlet basati sull'API REST e nettamente più performanti. Può essere un'ottima soluzione per molti CMDlet Get che vengono usati di frequente.
- Se è necessario usare CMDlet non coperti dal modulo v2, vedere l'argomento relativo all'[esecuzione di cmdlet di PowerShell per un numero elevato di utenti in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), che illustra come ovviare ai limiti di PowerShell in Exchange Online.
