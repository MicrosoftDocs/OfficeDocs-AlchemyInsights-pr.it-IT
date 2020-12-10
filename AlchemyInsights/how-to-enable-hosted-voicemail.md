---
title: Come abilitare la segreteria telefonica ospitata
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608848"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="ccebc-102">Come abilitare la segreteria telefonica ospitata</span><span class="sxs-lookup"><span data-stu-id="ccebc-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="ccebc-103">Per abilitare la segreteria telefonica, è necessario impostare **HostedVoicemail** su $true.</span><span class="sxs-lookup"><span data-stu-id="ccebc-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="ccebc-104">La proprietà **HostedVoicemail** dell'utente che utilizza Remote PowerShell (RPS).</span><span class="sxs-lookup"><span data-stu-id="ccebc-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="ccebc-105">Per ulteriori informazioni sulla connessione a RPS, vedere [Microsoft teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) per ulteriori informazioni sulla connessione a RPS.</span><span class="sxs-lookup"><span data-stu-id="ccebc-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="ccebc-106">È necessario che l'amministratore dei team sia connesso a Remote PowerShell per i team.</span><span class="sxs-lookup"><span data-stu-id="ccebc-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="ccebc-107">Dal prompt di PowerShell l'amministratore dei team può eseguire **set-csuser user@contoso.com-HostedVoiceMail $true** in cui l'URI SIP è dell'utente in questione.</span><span class="sxs-lookup"><span data-stu-id="ccebc-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="ccebc-108">Le modifiche apportate ai criteri possono richiedere fino a 24 ore per la replica.</span><span class="sxs-lookup"><span data-stu-id="ccebc-108">Changes to policies can take up to 24 hours to replicate.</span></span>