---
title: Impedire lo spostamento automatico dei messaggi nell'archivio
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736942"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a>Impedire lo spostamento automatico dei messaggi nell'archivio

Se si utilizza un criterio di conservazione, è possibile modificare il periodo di validità di conservazione in tale criterio per impedire l'archiviazione automatica dei messaggi. Ecco come:

1. [Nell'interfaccia di amministrazione di Exchange](https://go.microsoft.com/fwlink/?linkid=2059104)scegliere i tag di conservazione per la **gestione**  >  **della conformità.** Individuare il tag di conservazione Sposta nell'archivio.
2. Nel tag di conservazione modificare il periodo di conservazione (periodo di archiviazione) in **Mai** per impedire che gli elementi vengano archiviati automaticamente da un criterio di conservazione.

> [!NOTE]
> In questo modo verrà cambiata l'impostazione di archiviazione per tutte le cassette postali a cui è applicato questo tag di conservazione.
