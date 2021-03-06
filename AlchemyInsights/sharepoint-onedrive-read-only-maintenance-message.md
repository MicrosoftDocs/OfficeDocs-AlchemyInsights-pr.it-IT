---
title: Di sola lettura per il messaggio di manutenzione quando si tenta di utilizzare SharePoint o OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670836"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Di sola lettura per il messaggio di manutenzione quando si tenta di utilizzare SharePoint o OneDrive

Gli utenti possono ricevere un messaggio di **sola lettura per la manutenzione** quando si tenta di utilizzare SharePoint o OneDrive per uno degli scenari seguenti. 

-   Attività di manutenzione pianificata o attiva.  Verificarne la navigazione verso il [centro messaggi](https://portal.office.com/adminportal/home#/messagecenter).
-   Incidente di servizio attivo ad alta priorità che potrebbe verificarsi. Controllare se sono presenti avvisi o eventi indesiderati per l'esplorazione dell' [integrità del servizio](https://portal.office.com/adminportal/home#/servicehealth).
-   Uno scenario di ripristino di correzione automatica secondario che potrebbe verificarsi a causa di eventuali eventi imprevisti nei server che potrebbero durare meno di 30 minuti. 
    
    Non sono disponibili messaggi di centro messaggi o di integrità dei servizi per questi rilevamenti di minore entità, ma è consigliabile tornare alla normalità molto presto.

In pochissime occasioni è stato osservato che uno dei tre scenari sopra elencati è stato la causa e il servizio è stato ripristinato, ma la cache del browser degli utenti non è stata cancellata.

Provare a cancellare la cache del browser prima di passare al sito.

1. Nel browser Microsoft Edge, selezionare **Impostazioni**, quindi selezionare **privacy e sicurezza**.
2. In **Pulisci esplorazione**, seleziona **Scegli cosa cancellare**.
3. Selezionare **cookie e dati del sito Web salvati**e selezionare **Annulla**.

>[!Note] 
> Questa procedura può essere diversa quando si utilizzano altri browser come Mozilla Firefox o Google Chrome.

>[!Note] 
> Un'altra opzione consiste nell'aprire il sito di SharePoint o OneDrive in una nuova finestra di InPrivate.