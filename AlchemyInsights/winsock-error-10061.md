---
title: 1554 errore Winsock 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772446"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="d8812-102">Errore Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="d8812-102">Winsock error 10061</span></span>

<span data-ttu-id="d8812-103">Questo codice di errore indica che Office 365 non è stato in grado di stabilire un socket TCP (connessione) con l'host di destinazione.</span><span class="sxs-lookup"><span data-stu-id="d8812-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="d8812-104">La causa più probabile di questo errore è un problema con la configurazione del firewall.</span><span class="sxs-lookup"><span data-stu-id="d8812-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="d8812-105">Per risolvere il problema, controllare queste impostazioni:</span><span class="sxs-lookup"><span data-stu-id="d8812-105">To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="d8812-106">Verificare la configurazione del firewall con le informazioni negli [intervalli di indirizzi IP e URL di Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="d8812-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="d8812-107">Se l'errore è specifico di Exchange Online Protection (EOP), è necessario essere stati precedentemente informati di una modifica apportata agli [indirizzi IP di Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="d8812-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="d8812-108">Verificare che il provider di servizi Internet (ISP) non blocchi la porta.</span><span class="sxs-lookup"><span data-stu-id="d8812-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="d8812-109">Verificare le impostazioni di smart host e del server di destinazione nei connettori.</span><span class="sxs-lookup"><span data-stu-id="d8812-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="d8812-110">Si noti che Office 365 non blocca le connessioni in *ingresso* in questo modo.</span><span class="sxs-lookup"><span data-stu-id="d8812-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  
