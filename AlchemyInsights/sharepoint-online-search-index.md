---
title: Gestire i dizionari di ricerca in SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736057"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="b314e-102">Ricerca in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b314e-102">Search in SharePoint Online</span></span>

<span data-ttu-id="b314e-103">Il contenuto deve essere sottoposto a ricerca per indicizzazione e aggiunto all'indice di ricerca per consentire agli utenti di trovare ciò che stanno cercando in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b314e-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="b314e-104">Il contenuto viene sottoposto a ricerca per indicizzazione in base a una pianificazione di ricerca per indicizzazione predefinita (la pianificazione della ricerca per indicizzazione</span><span class="sxs-lookup"><span data-stu-id="b314e-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="b314e-105">Il crawler recupera il contenuto modificato dall'ultima ricerca per indicizzazione e aggiorna l'indice.</span><span class="sxs-lookup"><span data-stu-id="b314e-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="b314e-106">Per assicurarsi che il contenuto venga sottoposto a ricerca per indicizzazione e che l'indice venga aggiornato, eseguire la procedura seguente.</span><span class="sxs-lookup"><span data-stu-id="b314e-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="b314e-107">Verificare che il contenuto possa essere trovato facendo in modo che il contenuto del sito sia ricercabile.</span><span class="sxs-lookup"><span data-stu-id="b314e-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="b314e-108">Per altre informazioni, vedere [abilitare il contenuto di un sito per la ricerca](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="b314e-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="b314e-109">Quando si modifica una proprietà gestita o quando si modifica il mapping delle proprietà sottoposte a ricerca per indicizzazione o gestite, è necessario sottoporre di nuovo il sito a ricerca per indicizzazione per riflettere le modifiche nell'indice di ricerca.</span><span class="sxs-lookup"><span data-stu-id="b314e-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="b314e-110">Poiché le modifiche vengono apportate nello schema di ricerca e non nel sito effettivo, il crawler non reindicizzerà automaticamente il sito.</span><span class="sxs-lookup"><span data-stu-id="b314e-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="b314e-111">Per altre informazioni, vedere [ricerca per indicizzazione e reindicizzazione manuale di un sito, di una raccolta o di un elenco](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="b314e-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="b314e-112">Attendere almeno 24 ore dopo aver richiesto manualmente una ricerca per indicizzazione e una reindicizzazione completa per verificare se si è verificato un problema.</span><span class="sxs-lookup"><span data-stu-id="b314e-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="b314e-113">Se sono passate più di 24 ore da quando è stata avviata la ricerca per indicizzazione e la reindicizzazione completa, accedere a un caso di supporto.</span><span class="sxs-lookup"><span data-stu-id="b314e-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="b314e-114">In molti casi, stiamo già lavorando a una soluzione.</span><span class="sxs-lookup"><span data-stu-id="b314e-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b314e-115">Per completare una soluzione, è possibile fornirci almeno 24 ore.</span><span class="sxs-lookup"><span data-stu-id="b314e-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="b314e-116">**Importante**: se un sito, un documento (raccolta) o un elenco è stato eliminato e ancora viene visualizzato nei risultati di ricerca, gli utenti devono ricevere un file di errore 404 non trovato durante il tentativo di accesso.</span><span class="sxs-lookup"><span data-stu-id="b314e-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="b314e-117">Questo problema dovrebbe essere registrato come caso di supporto per ulteriori indagini.</span><span class="sxs-lookup"><span data-stu-id="b314e-117">This issue should be logged as a support case for further investigation.</span></span> 


