---
title: Il client di Teams si arresta in modo anomalo?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030683"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="a85b8-102">Il client di Teams si arresta in modo anomalo?</span><span class="sxs-lookup"><span data-stu-id="a85b8-102">Teams client crashing?</span></span>

<span data-ttu-id="a85b8-103">Se il client di Teams si arresta in modo anomalo, provare le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="a85b8-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="a85b8-104">Se si usa l'applicazione desktop di Teams, [verificare che l'app sia completamente aggiornata](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="a85b8-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="a85b8-105">Assicurarsi che tutti gli [intervalli di indirizzi e gli URL di Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) siano accessibili.</span><span class="sxs-lookup"><span data-stu-id="a85b8-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="a85b8-106">Eseguire l'accesso con l'account amministratore e controllare la [Dashboard di integrità dei servizi](https://docs.microsoft.com/office365/enterprise/view-service-health) per verificare che non siano presenti interruzioni o riduzioni delle prestazioni del servizio.</span><span class="sxs-lookup"><span data-stu-id="a85b8-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="a85b8-107">Come ultimo passaggio, si può provare a cancellare la cache del client di Teams:</span><span class="sxs-lookup"><span data-stu-id="a85b8-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="a85b8-108">Chiudere il client desktop di Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a85b8-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="a85b8-109">È possibile fare clic con il pulsante destro del mouse su **Teams** nell'area delle icone e fare clic su **Esci** o eseguire Gestione attività e arrestare completamente il processo.</span><span class="sxs-lookup"><span data-stu-id="a85b8-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="a85b8-110">Passare a Esplora file e digitare %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="a85b8-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="a85b8-111">Una volta nella directory, vengono visualizzate alcune delle seguenti cartelle:</span><span class="sxs-lookup"><span data-stu-id="a85b8-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="a85b8-112">All'interno di **Application Cache**, passare a Cache ed eliminare gli eventuali file presenti nel percorso di Cache: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="a85b8-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="a85b8-113">All'interno di **Blob_storage**, eliminare tutti i file: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="a85b8-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="a85b8-114">All'interno di **Cache**, eliminare tutti i file: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="a85b8-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="a85b8-115">All'interno di **databases**, eliminare tutti i file: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="a85b8-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="a85b8-116">All'interno di **GPUCache**, eliminare tutti i file: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="a85b8-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="a85b8-117">All'interno di **IndexedDB**, eliminare tutti i file .db: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="a85b8-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="a85b8-118">All'interno di **Local Storage**, eliminare tutti i file: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="a85b8-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="a85b8-119">Infine, all'interno di **tmp**, eliminare i file: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="a85b8-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="a85b8-120">Riavviare il client di Teams.</span><span class="sxs-lookup"><span data-stu-id="a85b8-120">Restart your Teams client.</span></span>
