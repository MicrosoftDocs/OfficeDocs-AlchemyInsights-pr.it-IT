---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770995"
---
# <a name="verify-your-domain"></a><span data-ttu-id="021ea-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="021ea-102">Verify your domain</span></span>

 <span data-ttu-id="021ea-103">**Il record probabilmente non è stato aggiornato su Internet.**</span><span class="sxs-lookup"><span data-stu-id="021ea-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="021ea-104">In genere ci vogliono pochi minuti per poter visualizzare il nuovo record, ma a volte possono essere necessari fino a poche ore.</span><span class="sxs-lookup"><span data-stu-id="021ea-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="021ea-105">Se l'attesa è già lunga, verificare di aver copiato e incollato il valore esatto nel record di verifica TXT nell'host DNS.</span><span class="sxs-lookup"><span data-stu-id="021ea-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="021ea-106">Un problema comune non include la parte "MS=" del record.</span><span class="sxs-lookup"><span data-stu-id="021ea-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="021ea-107">Abbiamo bisogno anche di questo!</span><span class="sxs-lookup"><span data-stu-id="021ea-107">We need that too!</span></span>

- <span data-ttu-id="021ea-108">Presso alcuni host DNS è necessario eseguire un ulteriore passaggio per salvare il file di zona (in cui è archiviato il record DNS) in modo che venga aggiornato su Internet.</span><span class="sxs-lookup"><span data-stu-id="021ea-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="021ea-109">Assicurarsi di aver salvato le modifiche in modo che Microsoft possa visualizzare e verificare il record.</span><span class="sxs-lookup"><span data-stu-id="021ea-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
