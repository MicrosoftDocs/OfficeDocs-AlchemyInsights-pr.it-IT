---
title: Risolvere i problemi comuni relativi alla formattazione dei record DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737176"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Risolvere i problemi comuni relativi alla formattazione dei record DKIM

La maggior parte dei problemi di configurazione di DKIM è correlata a record DNS non corretti.

Per risolvere i problemi di configurazione di DKIM, verificare che il record CNAME DKIM **(non** un record TXT) sia formattato correttamente. Per ulteriori informazioni, vedere [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Per assistenza generale con i record DNS, vedere [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Dopo aver creato o aggiornato i record DNS DKIM nel servizio di hosting DNS per il dominio, è necessario attendere la propagazione dei record DNS.
