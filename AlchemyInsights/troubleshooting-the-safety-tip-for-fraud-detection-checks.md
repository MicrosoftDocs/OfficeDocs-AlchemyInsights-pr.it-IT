---
title: Risoluzione dei problemi relativi al suggerimento per la sicurezza per i controlli di rilevamento delle frodi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834735"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="1cdaa-102">Risoluzione dei problemi relativi al suggerimento per la sicurezza per i controlli di rilevamento delle frodi</span><span class="sxs-lookup"><span data-stu-id="1cdaa-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="1cdaa-103">Se si riceve un suggerimento per la sicurezza che indica che il mittente non ha superato i controlli di rilevamento delle frodi e potrebbe non essere quello che sembra essere", il mittente non è riuscito a superare i controlli di autenticazione DKIM o SPF.</span><span class="sxs-lookup"><span data-stu-id="1cdaa-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="1cdaa-104">Il metodo migliore per risolvere il problema è che il mittente si autorizzi.</span><span class="sxs-lookup"><span data-stu-id="1cdaa-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="1cdaa-105">Se il mittente invia per conto dell'utente, è necessario autorizzarlo aggiungendo l'indirizzo IP del mittente al record SPF.</span><span class="sxs-lookup"><span data-stu-id="1cdaa-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="1cdaa-106">Vedi [Risoluzione dei problemi del suggerimento di sicurezza rosso (sospetto) per i controlli di rilevamento delle frodi](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) per altre info.</span><span class="sxs-lookup"><span data-stu-id="1cdaa-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="1cdaa-107">Ecco alcuni altri collegamenti utili:</span><span class="sxs-lookup"><span data-stu-id="1cdaa-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="1cdaa-108">Come Microsoft usa SPF (Sender Policy Framework) per impedire lo spoofing</span><span class="sxs-lookup"><span data-stu-id="1cdaa-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="1cdaa-109">Configurazione di SPF per evitare lo spoofing</span><span class="sxs-lookup"><span data-stu-id="1cdaa-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
