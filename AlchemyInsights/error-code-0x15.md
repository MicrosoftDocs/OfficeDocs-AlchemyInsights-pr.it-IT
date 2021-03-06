---
title: Codice di errore 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se si riceve un errore durante l'attivazione di Office 2013 nelle distribuzioni di Servizi Desktop remoto (RDS), è consigliabile abilitare ADAL modificando il registro di sistema.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709191"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Errore durante l'attivazione di Office 2013 su Servizi Desktop remoto

Se si riceve un errore durante l'attivazione di Office 2013 nelle distribuzioni di Servizi Desktop remoto (RDS), è consigliabile abilitare ADAL modificando il registro di sistema.
  
|**Chiave del Registro di sistema**|**Tipo**|**Valore**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |

Per ulteriori informazioni, vedere [abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL è abilitato per impostazione predefinita in Microsoft 365 Apps for Enterprise e Office 2016. I Servizi Desktop remoto (RDS) sono stati precedentemente denominati Servizi terminal.
  