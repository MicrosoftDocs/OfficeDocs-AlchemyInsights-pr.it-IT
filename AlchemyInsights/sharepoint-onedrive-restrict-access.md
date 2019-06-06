---
title: Limitare l'accesso in SharePoint o OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735147"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="0b845-102">Limitare l'accesso in SharePoint o OneDrive</span><span class="sxs-lookup"><span data-stu-id="0b845-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="0b845-103">Esistono diversi modi per limitare l'accesso ai servizi di SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0b845-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="0b845-104">Di seguito sono descritti i diversi metodi di restrizione di accesso.</span><span class="sxs-lookup"><span data-stu-id="0b845-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="0b845-105">Limitazione delle autorizzazioni</span><span class="sxs-lookup"><span data-stu-id="0b845-105">Permission Restriction</span></span>

<span data-ttu-id="0b845-106">In SharePoint Online e OneDrive for business, è possibile limitare l'accesso a elementi come siti, file e cartelle concedendo l'accesso solo ai gruppi/utenti che devono avere accesso.</span><span class="sxs-lookup"><span data-stu-id="0b845-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

[<span data-ttu-id="0b845-107">Personalizzare le autorizzazioni per un elenco o una raccolta di SharePoint</span><span class="sxs-lookup"><span data-stu-id="0b845-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[<span data-ttu-id="0b845-108">Personalizzare le autorizzazioni del sito di SharePoint</span><span class="sxs-lookup"><span data-stu-id="0b845-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[<span data-ttu-id="0b845-109">Modificare le autorizzazioni in una sottocartella</span><span class="sxs-lookup"><span data-stu-id="0b845-109">Change the permissions on a subfolder</span></span>](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[<span data-ttu-id="0b845-110">Controllare l'accesso da dispositivi non gestiti</span><span class="sxs-lookup"><span data-stu-id="0b845-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="0b845-111">In qualità di amministratore di SharePoint o globale in Office 365, è possibile bloccare o limitare l'accesso a SharePoint e il contenuto di OneDrive da dispositivi non gestiti (quelli non ibridi AD Uniti o conformi a Intune).</span><span class="sxs-lookup"><span data-stu-id="0b845-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="0b845-112">Limitazione del percorso di rete</span><span class="sxs-lookup"><span data-stu-id="0b845-112">Network Location Restriction</span></span>

<span data-ttu-id="0b845-113">In qualità di amministratore IT, è possibile controllare l'accesso alle risorse di SharePoint e OneDrive in base a percorsi di rete definiti attendibili.</span><span class="sxs-lookup"><span data-stu-id="0b845-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="0b845-114">Questo è noto anche come criterio basato sulla posizione.</span><span class="sxs-lookup"><span data-stu-id="0b845-114">This is also known as location-based policy.</span></span> <span data-ttu-id="0b845-115">Per ulteriori informazioni, vedere [controllare l'accesso ai dati di SharePoint Online e OneDrive in base al percorso di rete](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="0b845-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="0b845-116">Limitazione del blocco del sito</span><span class="sxs-lookup"><span data-stu-id="0b845-116">Site Lock Restriction</span></span> 

<span data-ttu-id="0b845-117">In SharePoint Online è possibile bloccare una raccolta siti, in modo che nessuno abbia accesso.</span><span class="sxs-lookup"><span data-stu-id="0b845-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="0b845-118">Questa impostazione viene impostata tramite PowerShell e [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) tramite la proprietà [set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="0b845-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="0b845-119">Impedire agli utenti di creare siti o sottositi</span><span class="sxs-lookup"><span data-stu-id="0b845-119">Restrict users from creating sites or subsites</span></span>

<span data-ttu-id="0b845-120">In qualità di amministratore di SharePoint o amministratore globale di Office 365, è possibile consentire agli utenti di creare e amministrare i propri siti di SharePoint, determinare il tipo di siti che possono creare e specificare il percorso dei siti.</span><span class="sxs-lookup"><span data-stu-id="0b845-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="0b845-121">Per ulteriori informazioni, vedere [gestire la creazione di siti in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="0b845-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span></span>
