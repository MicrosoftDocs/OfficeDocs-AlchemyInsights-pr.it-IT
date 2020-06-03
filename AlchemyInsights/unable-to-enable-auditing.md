---
title: 2419-Impossibile-attivare-controllo
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510432"
---
# <a name="unable-to-enable-unified-auditing"></a>Impossibile abilitare il controllo unificato

Quando si tenta di abilitare il controllo unificato per l'organizzazione, è possibile che venga visualizzato un errore simile al seguente:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Per risolvere il problema, attenersi alla seguente procedura:

1. [Connettersi a PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Eseguire il seguente cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Attendere 60 minuti per rendere effettive le impostazioni precedenti.

4. Eseguire il seguente comando in PowerShell di Exchange Online:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Per ulteriori informazioni, vedere gli articoli seguenti:

- [Connettersi a PowerShell di Exchange Online utilizzando l'autenticazione a più fattori](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Abilitare o disabilitare la ricerca nel log di controllo](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
