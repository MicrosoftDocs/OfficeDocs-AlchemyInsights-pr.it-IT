---
title: Attivare il controllo delle cassette postali
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464937"
---
# <a name="turn-on-mailbox-auditing"></a>Attivare il controllo delle cassette postali

Per attivare il controllo delle cassette postali per un singolo utente o un'intera organizzazione, eseguire i cmdlet seguenti da Remote PowerShell:

- **Utente singolo**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **Organizzazione**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Per ulteriori informazioni, vedere [Gestire il controllo delle cassette postali.](https://go.microsoft.com/fwlink/?linkid=2103668)