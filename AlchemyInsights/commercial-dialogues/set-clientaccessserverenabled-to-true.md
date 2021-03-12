---
title: Impostare ClientAccessServerEnabled su True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736990"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="b087e-102">Impostare ClientAccessServerEnabled su True</span><span class="sxs-lookup"><span data-stu-id="b087e-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="b087e-103">Se non è possibile aprire un messaggio di posta elettronica crittografato e visualizzare invece un allegato **rpmsg,** eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="b087e-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="b087e-104">Connettersi a PowerShell di Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="b087e-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="b087e-105">Per connettersi a PowerShell di Exchange Online, è necessario accedere utilizzando un account di amministratore globale o di amministratore di Exchange.</span><span class="sxs-lookup"><span data-stu-id="b087e-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="b087e-106">a.</span><span class="sxs-lookup"><span data-stu-id="b087e-106">a.</span></span> <span data-ttu-id="b087e-107">Aprire Windows PowerShell ed eseguire il comando seguente: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="b087e-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="b087e-108">b.</span><span class="sxs-lookup"><span data-stu-id="b087e-108">b.</span></span> <span data-ttu-id="b087e-109">Nella finestra **Windows PowerShell richiesta credenziali** immettere l'account aziendale o dell'istituto di istruzione e la password, c.</span><span class="sxs-lookup"><span data-stu-id="b087e-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="b087e-110">Fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="b087e-110">Click **OK**.</span></span> 

2. <span data-ttu-id="b087e-111">Eseguire il comando seguente per creare una nuova sessione:</span><span class="sxs-lookup"><span data-stu-id="b087e-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="b087e-112">a.</span><span class="sxs-lookup"><span data-stu-id="b087e-112">a.</span></span> <span data-ttu-id="b087e-113">Eseguire il comando seguente:</span><span class="sxs-lookup"><span data-stu-id="b087e-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="b087e-114">Eseguire `Get-IRMConfiguration` il comando.</span><span class="sxs-lookup"><span data-stu-id="b087e-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="b087e-115">Controllare **l'impostazione ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="b087e-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="b087e-116">a.</span><span class="sxs-lookup"><span data-stu-id="b087e-116">a.</span></span> <span data-ttu-id="b087e-117">Se **l'impostazione ClientAccessServerEnabled** è impostata su **False,** eseguire il cmdlet seguente: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="b087e-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="b087e-118">Chiudi sempre la sessione di PowerShell con il comando seguente: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="b087e-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="b087e-119">Per ulteriori informazioni, vedere [PowerShell di Exchange Online.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="b087e-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

