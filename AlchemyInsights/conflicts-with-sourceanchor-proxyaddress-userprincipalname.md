---
title: Conflitti con SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 877c954bea219cf8d885645cd25e41a5b7bab6fd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713458"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a>Conflitti con SourceAnchor, ProxyAddress, UserPrincipalName

Se durante una sincronizzazione si ricevono errori simili a "Nella directory esiste già un oggetto sincronizzato con lo stesso valore di ProxyAddress o UserPrincipalName", vedere [Diagnosticare e risolvere gli errori di sincronizzazione degli attributi duplicati](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).

Inoltre, è consigliabile abilitare la resilienza degli attributi duplicati. Per altre informazioni, vedere [Sincronizzazione delle identità e resilienza degli attributi duplicati](https://aka.ms/duplicateattributeresiliency).