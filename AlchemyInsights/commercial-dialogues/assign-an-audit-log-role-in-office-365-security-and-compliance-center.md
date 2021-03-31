---
title: Assegnare un ruolo del log di audit nel Centro sicurezza e conformità di Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736849"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="f8aee-102">Assegnare un ruolo del log di audit nel Centro sicurezza e conformità di Office 365</span><span class="sxs-lookup"><span data-stu-id="f8aee-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="f8aee-103">Per eseguire ricerche nel log di controllo di Office 365, è necessario che a un amministratore sia stato assegnato il ruolo relativo ai **Log di audit di sola lettura** o il ruolo relativo ai **Log di audit** in Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f8aee-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="f8aee-104">Questi ruoli vengono assegnati ai gruppi di ruoli Gestione conformità e Gestione organizzazione per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="f8aee-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="f8aee-105">Gli amministratori globali di Office 365 e Microsoft 365 vengono aggiunti automaticamente come membri del gruppo di ruoli Gestione organizzazione.</span><span class="sxs-lookup"><span data-stu-id="f8aee-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="f8aee-106">Per abilitare un utente a eseguire ricerche con il livello minimo di privilegi, creare un gruppo di ruoli personalizzato in Exchange Online, aggiungere il ruolo relativo ai **Log di controllo di sola lettura** o ai **Log di controllo** e quindi aggiungere l'utente come membro del nuovo gruppo di ruoli.</span><span class="sxs-lookup"><span data-stu-id="f8aee-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="f8aee-107">Per altre informazioni, vedere [Gestire i gruppi di ruoli in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) e [Eseguire ricerche nel log di controllo nel Centro sicurezza e conformità](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="f8aee-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>