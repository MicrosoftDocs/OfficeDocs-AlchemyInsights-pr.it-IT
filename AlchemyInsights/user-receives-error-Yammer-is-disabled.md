---
title: L'utente riceve l'errore AADSTS7000112 Yammer is disabled
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157338"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="2fd08-102">L'utente riceve l'errore AADSTS7000112 Yammer is disabled</span><span class="sxs-lookup"><span data-stu-id="2fd08-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="2fd08-103">Se si riceve il messaggio di errore "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", si è verificato un problema con l'entità servizio in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2fd08-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="2fd08-104">Un amministratore potrebbe aver disabilitato l'entità servizio per bloccare l'accesso a Yammer.</span><span class="sxs-lookup"><span data-stu-id="2fd08-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="2fd08-105">La disabilitazione dell'entità servizio non è consigliata e può causare altri problemi.</span><span class="sxs-lookup"><span data-stu-id="2fd08-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="2fd08-106">Per altre informazioni sull'approccio supportato per bloccare l'accesso degli utenti a Yammer, vedere [Disattivare l'accesso Yammer per gli utenti di Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="2fd08-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="2fd08-107">Per risolvere il problema nel portale di Azure e ripristinare l'accesso degli utenti a Yammer:</span><span class="sxs-lookup"><span data-stu-id="2fd08-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="2fd08-108">Aprire la pagina di Azure Active Directory e selezionare **Applicazioni aziendali** in **Gestisci** nel riquadro di spostamento sinistro.</span><span class="sxs-lookup"><span data-stu-id="2fd08-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="2fd08-109">Digitare **Office 365 Yammer** nella casella di ricerca e selezionare il nome dell'applicazione per aprire le impostazioni.</span><span class="sxs-lookup"><span data-stu-id="2fd08-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="2fd08-110">Selezionare **Proprietà** in **Gestisci** nel riquadro di spostamento sinistro.</span><span class="sxs-lookup"><span data-stu-id="2fd08-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="2fd08-111">Impostare il valore **Abilitato per l'accesso degli utenti?** su **Sì**, quindi selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="2fd08-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="2fd08-112">Accedere nuovamente a Yammer.</span><span class="sxs-lookup"><span data-stu-id="2fd08-112">Sign in to Yammer again.</span></span> <span data-ttu-id="2fd08-113">Potrebbe essere necessario cancellare i cookie.</span><span class="sxs-lookup"><span data-stu-id="2fd08-113">You might need to clear cookies.</span></span>

<span data-ttu-id="2fd08-114">In alternativa, eseguire i comandi di PowerShell per impostare il valore.</span><span class="sxs-lookup"><span data-stu-id="2fd08-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="2fd08-115">Per ulteriori informazioni, vedere [Errore "Sorry, but we're having trouble signing you in" quando si fa clic sul riquadro di Yammer in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="2fd08-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 