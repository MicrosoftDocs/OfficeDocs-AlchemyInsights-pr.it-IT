---
title: Correggere le regole di trasporto
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737134"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="0b4a7-102">Correggere le regole di trasporto</span><span class="sxs-lookup"><span data-stu-id="0b4a7-102">Fix transport rules</span></span>

<span data-ttu-id="0b4a7-103">Questo messaggio è stato influenzato da una regola del flusso di posta personalizzata.</span><span class="sxs-lookup"><span data-stu-id="0b4a7-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="0b4a7-104">Per esaminare la regola esatta, eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="0b4a7-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="0b4a7-105">Nei risultati dell'invio, in **Ulteriori informazioni,** prendere nota del **GUID** o del **nome del criterio.**</span><span class="sxs-lookup"><span data-stu-id="0b4a7-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="0b4a7-106">Avviare Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="0b4a7-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="0b4a7-107">Per ulteriori informazioni, vedere [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="0b4a7-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="0b4a7-108">Eseguire questo comando (usando il GUID dall'invio):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="0b4a7-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="0b4a7-109">Esaminare la descrizione per visualizzare le condizioni configurate che hanno interessato il messaggio.</span><span class="sxs-lookup"><span data-stu-id="0b4a7-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="0b4a7-110">Per ulteriori informazioni, vedere [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="0b4a7-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>