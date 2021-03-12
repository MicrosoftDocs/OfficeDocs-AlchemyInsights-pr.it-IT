---
title: Criteri per le password
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718204"
---
# <a name="password-policies"></a><span data-ttu-id="67eeb-102">Criteri per le password</span><span class="sxs-lookup"><span data-stu-id="67eeb-102">Password policies</span></span>

<span data-ttu-id="67eeb-103">**I'm having problems with the password policy for a user**</span><span class="sxs-lookup"><span data-stu-id="67eeb-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="67eeb-104">I criteri password per un utente dipendono dal fatto che l'utente sia solo cloud o locale.</span><span class="sxs-lookup"><span data-stu-id="67eeb-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="67eeb-105">Gli utenti solo cloud devono scegliere una password che soddisfi i requisiti riportati in questo articolo: Criteri per le password che si applicano solo [agli account utente cloud](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="67eeb-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="67eeb-106">Gli utenti locali devono scegliere una password che soddisfi i requisiti locali.</span><span class="sxs-lookup"><span data-stu-id="67eeb-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="67eeb-107">Se un utente locale non è in grado di impostare la password, controllare i requisiti locali.</span><span class="sxs-lookup"><span data-stu-id="67eeb-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="67eeb-108">**Non so come impostare o controllare i criteri di scadenza delle password**</span><span class="sxs-lookup"><span data-stu-id="67eeb-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="67eeb-109">È possibile impostare e controllare i criteri di scadenza per gli utenti cloud nel tenant tramite PowerShell.</span><span class="sxs-lookup"><span data-stu-id="67eeb-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="67eeb-110">Seguire le istruzioni in questo articolo: [Impostare o controllare i criteri password tramite PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="67eeb-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="67eeb-111">I criteri di scadenza delle password per gli utenti locali sono impostati in Active Directory locale.</span><span class="sxs-lookup"><span data-stu-id="67eeb-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="67eeb-112">**Altri collegamenti utili:**</span><span class="sxs-lookup"><span data-stu-id="67eeb-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="67eeb-113">Introduzione alla reimpostazione della password</span><span class="sxs-lookup"><span data-stu-id="67eeb-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="67eeb-114">Risoluzione dei problemi relativi alla reimpostazione della password avviata dall'amministratore</span><span class="sxs-lookup"><span data-stu-id="67eeb-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
