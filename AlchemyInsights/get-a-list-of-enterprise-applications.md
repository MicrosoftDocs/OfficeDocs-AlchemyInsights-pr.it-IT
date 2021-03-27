---
title: Ottenere un elenco di applicazioni aziendali
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379850"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="924c8-102">Ottenere un elenco di applicazioni aziendali</span><span class="sxs-lookup"><span data-stu-id="924c8-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="924c8-103">Per **ottenere un elenco** di applicazioni aziendali (tutte le applicazioni o filtrate per nome visualizzato, ID, URI identificatore e così via) tramite il comando powershell, vedere [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="924c8-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="924c8-104">Per ottenere un elenco di oggetti entità servizio (tutti gli oggetti o filtrati in base all'ID) tramite il comando powershell, vedere [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="924c8-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="924c8-105">Se si desidera ottenere **un elenco delle app configurate saml, gli script di PowerShell** seguenti possono essere utili:</span><span class="sxs-lookup"><span data-stu-id="924c8-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="924c8-106">Ogni applicazione che si tratta di un'app OAuth o SAML (sia app di raccolta che di app non di raccolta) avrebbe due oggetti creati in AAD quando viene eseguita la registrazione.</span><span class="sxs-lookup"><span data-stu-id="924c8-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="924c8-107">Uno è denominato oggetto Application e l'altro è l'oggetto Entità servizio.</span><span class="sxs-lookup"><span data-stu-id="924c8-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="924c8-108">Quando si esegue il dump delle proprietà di un oggetto entità servizio tramite PowerShell, si scoprirebbe che a ogni applicazione è associato un determinato numero di tag, ad esempio:</span><span class="sxs-lookup"><span data-stu-id="924c8-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="924c8-109">Le app OAuth avrebbero un tag denominato "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="924c8-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="924c8-110">Raccolta App SAML con un tag denominato "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="924c8-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="924c8-111">Le app SAML non della raccolta avrebbero un tag denominato "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="924c8-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="924c8-112">Di conseguenza, puoi usare questi tag e scoprire che tipo di app si tratta.</span><span class="sxs-lookup"><span data-stu-id="924c8-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="924c8-113">Il tag "**WindowsAzureActiveDirectoryIntegratedApp**" è comune a tutti i tipi di app.</span><span class="sxs-lookup"><span data-stu-id="924c8-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="924c8-114">Puoi usare il frammento di codice seguente per elencare tutte le app SAML (sia raccolta che non raccolta):</span><span class="sxs-lookup"><span data-stu-id="924c8-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="924c8-115">Per altre informazioni, vedi [Identificare le app abilitate per SAML in Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="924c8-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="924c8-116">**Trovare ed elencare solo le applicazioni Web:** utilizzare il comando seguente per ottenere tutte le applicazioni di Azure AD con il tipo di applicazione "App Web/API"</span><span class="sxs-lookup"><span data-stu-id="924c8-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="924c8-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="924c8-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="924c8-118">**Trovare ed elencare solo le** applicazioni native: eseguire il comando seguente per ottenere tutte le applicazioni client native (desktop/dispositivo mobile).</span><span class="sxs-lookup"><span data-stu-id="924c8-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="924c8-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="924c8-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="924c8-120">**Export All Registered Azure AD Application Details to CSV**: Il comando seguente esporta tutte le app di Azure AD con i dettagli necessari in un file CSV:</span><span class="sxs-lookup"><span data-stu-id="924c8-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="924c8-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="924c8-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="924c8-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="924c8-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="924c8-123">**Necessità di esportare un elenco di app di Azure inutilizzate** - Report di controllo</span><span class="sxs-lookup"><span data-stu-id="924c8-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="924c8-124">Azure AD può visualizzare i log delle applicazioni solo per un massimo di 30 giorni, purché si abbia una licenza di Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="924c8-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="924c8-125">Sono disponibili due opzioni per conservare i dati per più di 30 giorni.</span><span class="sxs-lookup"><span data-stu-id="924c8-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="924c8-126">Puoi usare le [API per la creazione di report](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) di Azure AD per recuperare i dati a livello di programmazione e archiviarli in un database.</span><span class="sxs-lookup"><span data-stu-id="924c8-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="924c8-127">In alternativa, è possibile integrare i log di controllo in un sistema SIEM di terze parti.</span><span class="sxs-lookup"><span data-stu-id="924c8-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="924c8-128">Puoi anche scaricare l'elenco delle app per tutte le applicazioni e le applicazioni di proprietà in Azure Active directory>App Registrations>Download>Tutte le applicazioni/Applicazioni di proprietà.</span><span class="sxs-lookup"><span data-stu-id="924c8-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="924c8-129">Per ottenere un elenco delle applicazioni tramite MS Graph, vedere [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and application resource type - Microsoft Graph [v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="924c8-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
