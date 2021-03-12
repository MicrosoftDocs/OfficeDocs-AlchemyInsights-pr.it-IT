---
title: Offboard di dispositivi non Windows da Microsoft Defender Advanced Threat Protection (ATP)
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
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736539"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="8f3b1-102">Offboard di dispositivi non Windows da Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="8f3b1-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="8f3b1-103">Ecco come:</span><span class="sxs-lookup"><span data-stu-id="8f3b1-103">Here's how:</span></span>

1. <span data-ttu-id="8f3b1-104">Seguire la documentazione di terze parti per disconnettere la soluzione di terze parti da Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="8f3b1-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="8f3b1-105">Dal tenant di Azure Active Directory, rimuovere le autorizzazioni per la soluzione di terze parti:</span><span class="sxs-lookup"><span data-stu-id="8f3b1-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="8f3b1-106">Accedere al [portale di Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="8f3b1-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="8f3b1-107">Selezionare **Tutti i servizi** Azure Active  >  **Directory** Enterprise  >  **Applications**.</span><span class="sxs-lookup"><span data-stu-id="8f3b1-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="8f3b1-108">Seleziona l'applicazione che vuoi offboard.</span><span class="sxs-lookup"><span data-stu-id="8f3b1-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="8f3b1-109">Selezionare **Elimina**.</span><span class="sxs-lookup"><span data-stu-id="8f3b1-109">Select **Delete**.</span></span>

<span data-ttu-id="8f3b1-110">Per altre informazioni, vedi [Offboard non Windows devices.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="8f3b1-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
