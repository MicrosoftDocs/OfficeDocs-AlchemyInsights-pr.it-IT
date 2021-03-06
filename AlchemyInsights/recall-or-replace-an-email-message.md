---
title: Richiamare o sostituire un messaggio di posta elettronica
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353510"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Richiamare o sostituire un messaggio di posta elettronica in Microsoft 365

- È possibile **richiamare solo i messaggi inviati alle persone all'interno dell'organizzazione**. Ad esempio, se il messaggio è stato inviato a un indirizzo Gmail, non è possibile richiamarlo.
- È possibile **richiamare solo i messaggi inviati da Outlook per il PC**. Se un utente invia un messaggio utilizzando Outlook per Mac o Outlook sul Web, non è possibile richiamarlo.
- In qualità di amministratore tenant, è possibile **richiamare i messaggi per conto degli utenti utilizzando PowerShell** (per ulteriori informazioni, vedere: [cercare ed eliminare i messaggi di posta elettronica](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Non è possibile richiamare messaggi dall'interfaccia di amministrazione. Scorrere verso il basso fino a "cercare ed eliminare i messaggi di posta elettronica nell'organizzazione" per ulteriori informazioni.

**Richiamare o sostituire un messaggio di posta elettronica inviato**

1. Nel riquadro delle cartelle nella parte sinistra della finestra di Outlook scegliere la cartella posta inviata.
2. Aprire il messaggio che si desidera richiamare. È necessario fare doppio clic per aprire il messaggio. Se si seleziona il messaggio in modo che venga visualizzato nel riquadro di lettura, non sarà possibile richiamare il messaggio.
3. Nella scheda messaggio, selezionare **azioni**  >  **richiamare questo messaggio**.
4. Scegliere **Elimina copie non lette del messaggio** o **Elimina copie non lette e Sostituisci con un nuovo messaggio**, quindi selezionare **OK**.
5. Se si sta inviando un messaggio di sostituzione, comporre il messaggio, quindi selezionare **Invia**.
6. L'esito positivo o negativo di un messaggio di richiamo dipende dalle impostazioni dei destinatari in Outlook.

Per ulteriori informazioni, tra cui la verifica del richiamo, vedere [Recall or Replace an email message you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_Per cercare ed eliminare i messaggi di posta elettronica nell'organizzazione_**, è più semplice se si è un amministratore globale. Se non si è un amministratore globale, è necessario aggiungere l'account al gruppo di ruoli di eDiscovery Manager o al ruolo di gestione della ricerca di conformità. Per eliminare i messaggi, è necessario aggiungere il gruppo di ruoli Gestione organizzazione o il ruolo di gestione ricerca e Purge. Le autorizzazioni per questi ruoli vengono assegnate al [Centro sicurezza & Compliance](https://protection.office.com/).

1. [Creare una ricerca di contenuto](https://docs.microsoft.com/microsoft-365/compliance/content-search) per trovare il messaggio da eliminare.
2. [Connettersi a PowerShell in Centro sicurezza e conformità](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Se si utilizza l'autenticazione a più fattori, vedere [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
