---
title: La cartella RecoverableItems 1336 è piena
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: b8b3e5389778b3aff0fbe2f6506ba2b2fc3abc7e
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655671"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="40f92-102">La cartella elementi ripristinabili è piena</span><span class="sxs-lookup"><span data-stu-id="40f92-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="40f92-p101">Per cassette postali di Exchange Online in Office 365, il limite di archiviazione predefinito per la cartella elementi ripristinabili è 30 GB. Il limite di archiviazione per la cartella elementi recuperabili viene aumentato a 100 GB automaticamente se la cassetta postale viene messa in attesa di conservazione per controversia, esenzione di eDiscovery, o viene assegnata a un criterio di conservazione di Office 365.</span><span class="sxs-lookup"><span data-stu-id="40f92-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="40f92-105">Quando la cartella elementi ripristinabili raggiunge il limite di archiviazione, la funzionalità cassette postali interessata nei modi seguenti:</span><span class="sxs-lookup"><span data-stu-id="40f92-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="40f92-106">L'utente non può eliminare gli elementi dalla cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="40f92-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="40f92-107">Assistente cartelle gestite non può eliminare elementi basandosi sul tag di conservazione o sulle impostazioni delle cartelle gestite.</span><span class="sxs-lookup"><span data-stu-id="40f92-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="40f92-108">Per le cassette postali che dispongono di ripristino di un elemento singolo abilitato o messa in attesa, processo di protezione della pagina copia in scrittura non può mantenere le versioni di elementi modificati dall'utente.</span><span class="sxs-lookup"><span data-stu-id="40f92-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="40f92-109">Per le cassette postali con cassetta postale abilitata la registrazione di controllo, nessuna voce di registro di controllo delle cassette postali possono essere salvata nella sottocartella audit nella cartella elementi ripristinabili.</span><span class="sxs-lookup"><span data-stu-id="40f92-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="40f92-p102">Per le cassette postali che non sono in attesa, gli amministratori possono usare il `Search-Mailbox -SearchDumpsterOnly -DeleteContent` comando in Exchange Online PowerShell per eliminare gli elementi nella cartella elementi ripristinabili. Per ulteriori informazioni, vedere gli argomenti seguenti:</span><span class="sxs-lookup"><span data-stu-id="40f92-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="40f92-112">Cercare ed eliminare i messaggi</span><span class="sxs-lookup"><span data-stu-id="40f92-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="40f92-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="40f92-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="40f92-p103">Per le cassette postali che sono in attesa, è necessario rimuovere la conservazione prima che è possibile gli elementi eliminati dalla cartella elementi ripristinabili admins. Per ulteriori informazioni, vedere [eliminazione di elementi nella cartella delle cassette postali basate su cloud in attesa agli elementi ripristinabili](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="40f92-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="40f92-p104">Per evitare la cartella elementi recuperabili di diventare completa, gli amministratori possono aumentare il limite di archiviazione degli elementi recuperabili cartella delle cassette postali in attesa e configurare un criterio di conservazione delle cassette postali che sposta gli elementi dalla cartella elementi ripristinabili archivio dell'utente cassetta postale. Vedere [aumentare la quota per le cassette postali in attesa agli elementi ripristinabili](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="40f92-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

