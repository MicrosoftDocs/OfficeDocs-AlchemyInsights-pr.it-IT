---
title: Creare e condividere calendari di cartelle pubbliche in Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: bec11baa2de7154481ec175df2466eb601b0e243
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903581"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="5072b-102">Creare e condividere calendari di cartelle pubbliche in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5072b-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="5072b-103">È possibile creare un calendario nella cartella pubblica solo dal client desktop di Outlook.</span><span class="sxs-lookup"><span data-stu-id="5072b-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="5072b-104">Seguire questa procedura per configurare i calendari delle cartelle pubbliche:</span><span class="sxs-lookup"><span data-stu-id="5072b-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="5072b-105">Assicurarsi che le cartelle pubbliche siano distribuite in Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5072b-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="5072b-106">Per altre informazioni, vedere [creare una cassetta postale di cartelle pubbliche](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span><span class="sxs-lookup"><span data-stu-id="5072b-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="5072b-107">Assicurarsi che siano state assegnate le autorizzazioni di accesso necessarie per la creazione della cartella pubblica.</span><span class="sxs-lookup"><span data-stu-id="5072b-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="5072b-108">Per altre informazioni, vedere [autorizzazioni per le cartelle pubbliche per Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="5072b-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="5072b-109">Accedere al client desktop di Outlook e verificare che sia possibile accedere alla distribuzione delle cartelle pubbliche.</span><span class="sxs-lookup"><span data-stu-id="5072b-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="5072b-110">Se si verificano problemi durante l'accesso alle cartelle pubbliche con il client desktop di Outlook, vedere [Gli utenti di Exchange Online non possono connettersi alle cartelle pubbliche utilizzando Outlook o OWA](https://aka.ms/pfcte).</span><span class="sxs-lookup"><span data-stu-id="5072b-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="5072b-111">Creare un nuovo tipo di calendario per le cartelle pubbliche.</span><span class="sxs-lookup"><span data-stu-id="5072b-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="5072b-112">Per impostazione predefinita, la cartella pubblica viene condivisa con tutti gli altri utenti.</span><span class="sxs-lookup"><span data-stu-id="5072b-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="5072b-113">Il proprietario della cartella pubblica può cambiare le autorizzazioni dal client desktop di Outlook.</span><span class="sxs-lookup"><span data-stu-id="5072b-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="5072b-114">Per altre informazioni, vedere [autorizzazioni per le cartelle pubbliche per Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="5072b-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="5072b-115">**Nota:** i calendari delle cartelle pubbliche sono destinati all'uso all'interno dell'organizzazione e non possono essere pubblicati su Internet.</span><span class="sxs-lookup"><span data-stu-id="5072b-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="5072b-116">Usare una cassetta postale condivisa se si intende pubblicare un calendario su Internet.</span><span class="sxs-lookup"><span data-stu-id="5072b-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>