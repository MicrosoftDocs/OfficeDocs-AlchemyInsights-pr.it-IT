---
title: Eliminare un utente isolato da un server locale
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186131"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Eliminare un utente isolato da un server locale

Per rimuovere un utente isolato, procedere come segue:

1. Forzare la sincronizzazione della directory seguendo le istruzioni in [Che cos'è l'identità ibrida con Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Per verificare la sincronizzazione della directory, vedere [Che cos'è l'identità ibrida con Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Se la sincronizzazione funziona correttamente, ma l'eliminazione dell'oggetto di Active Directory non viene propagata in Azure AD, rimuovere manualmente l'oggetto isolato usando uno dei cmdlet seguenti del modulo Azure Active Directory per Windows PowerShell:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Ad esempio, per rimuovere l'ID utente isolato john.smith@contoso.com, creato in origine con la sincronizzazione della directory, eseguire il cmdlet:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com