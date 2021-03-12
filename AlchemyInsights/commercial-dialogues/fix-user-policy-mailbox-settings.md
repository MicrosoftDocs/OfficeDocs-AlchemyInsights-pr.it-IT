---
title: Correggere le impostazioni dei criteri utente/delle cassette postali
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737131"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="ce2d3-102">Correggere le impostazioni dei criteri utente/delle cassette postali</span><span class="sxs-lookup"><span data-stu-id="ce2d3-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="ce2d3-103">Le impostazioni della posta indesiderata nella cassetta postale hanno interessato questo messaggio.</span><span class="sxs-lookup"><span data-stu-id="ce2d3-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="ce2d3-104">Per esaminare le impostazioni, eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="ce2d3-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="ce2d3-105">Avviare Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="ce2d3-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="ce2d3-106">Per ulteriori informazioni, vedere [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="ce2d3-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="ce2d3-107">Eseguire questo comando (utilizzando l'indirizzo di posta elettronica dell'utente):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="ce2d3-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="ce2d3-108">Verificare se l'indirizzo di posta elettronica del mittente fa parte di **TrustedSendersAndDomains** **o BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="ce2d3-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="ce2d3-109">Se l'indirizzo di posta elettronica è in uno degli elenchi, potrebbe essere necessario rimuoverlo.</span><span class="sxs-lookup"><span data-stu-id="ce2d3-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="ce2d3-110">Per ulteriori informazioni, vedere [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="ce2d3-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
