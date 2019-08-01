---
title: Problemi di accesso alle app di Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938254"
---
# <a name="issues-signing-in-to-office-apps"></a>Problemi di accesso alle app di Office

Per risolvere i problemi di accesso con le app di Office, provare a eseguire le operazioni seguenti:

- Rimuovere tutti gli account di lavoro, ad eccezione dell'account danneggiato, utilizzando le impostazioni di Windows > **accedere al lavoro o all'Istituto di istruzione**.
- [Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.<br/>
    **Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0. (Es: \Software\Microsoft\Office\16.0\Common\Identity\)
- Aprire un'app di Office, scegliere**Esci dall'****account** >  **file** > . Accedere quindi utilizzando un account utente con una licenza valida. Per informazioni dettagliate, vedere [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Per Mac, vedere [Impossibile accedere a un'app di Office 2016 per Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Se si verificano errori durante la connessione a Office 365 con Office 2013, abilitare l'autenticazione moderna per il client di Office.

Per ulteriori informazioni, vedere:
- [Non è possibile accedere a Office 365, Azure o Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Problemi di connessione in accesso dopo l'aggiornamento a Office 2016 Build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Spiacenti, un altro account dell'organizzazione è già stato eseguito l'accesso al computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Risoluzione dei problemi di accesso con l'autenticazione moderna di Office quando si utilizzano ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)