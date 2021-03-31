---
title: Configurare e convalidare le esclusioni per MDATP in un computer Linux
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736766"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="58aa4-102">Configurare e convalidare le esclusioni per MDATP in un computer Linux</span><span class="sxs-lookup"><span data-stu-id="58aa4-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="58aa4-103">È possibile escludere determinati file, cartelle, processi e file aperti dal processo dalle analisi MDATP.</span><span class="sxs-lookup"><span data-stu-id="58aa4-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="58aa4-104">Le esclusioni impediscono il rilevamento errato di software e file univoci o personalizzati per l'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="58aa4-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="58aa4-105">Le esclusioni consentono inoltre di ridurre i problemi di prestazioni causati da MDATP.</span><span class="sxs-lookup"><span data-stu-id="58aa4-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="58aa4-106">Per altre informazioni, vedi [Configurare e convalidare le esclusioni per MDATP per Linux.](https://go.microsoft.com/fwlink/?linkid=2144517)</span><span class="sxs-lookup"><span data-stu-id="58aa4-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="58aa4-107">Le esclusioni descritte in questo articolo non si applicano ad altre funzionalità di MDATP per Linux, tra cui il rilevamento e la risposta degli endpoint (EDR).</span><span class="sxs-lookup"><span data-stu-id="58aa4-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="58aa4-108">I file esclusi utilizzando i metodi descritti in questo articolo possono comunque attivare avvisi EDR e altre funzionalità di rilevamento.</span><span class="sxs-lookup"><span data-stu-id="58aa4-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>