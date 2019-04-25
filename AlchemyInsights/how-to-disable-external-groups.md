---
title: Come disabilitare i gruppi esterni
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399667"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="24d64-102">Come disabilitare i gruppi esterni</span><span class="sxs-lookup"><span data-stu-id="24d64-102">How to disable External Groups</span></span>

<span data-ttu-id="24d64-103">La messaggistica esterna di Yammer applica le regole di trasporto di Exchange (ETRs), un insieme di controlli proattivi che impediscono la condivisione delle informazioni aziendali.</span><span class="sxs-lookup"><span data-stu-id="24d64-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="24d64-104">Per impedire agli utenti di creare gruppi esterni, è necessario configurare una regola di trasporto di Exchange (ETR), quindi configurare Yammer in modo da utilizzare la regola di trasporto di Exchange per bloccare la messaggistica esterna.</span><span class="sxs-lookup"><span data-stu-id="24d64-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="24d64-105">Dopo aver creato una regola nell'interfaccia di amministrazione di Exchange Online, eseguire la procedura seguente per impostare ETR per l'applicazione in Yammer:</span><span class="sxs-lookup"><span data-stu-id="24d64-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="24d64-106">Accedere a Yammer come amministratore verificato e, nell'interfaccia di **amministrazione di Yammer**, passare a C ontent e alle impostazioni di sicurezza di **sicurezza \> .**</span><span class="sxs-lookup"><span data-stu-id="24d64-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="24d64-107">In **messaggi esterni**selezionare **applica le regole di trasporto di Exchange Online (ETRs) in Yammer.**</span><span class="sxs-lookup"><span data-stu-id="24d64-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="24d64-108">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="24d64-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="24d64-109">Per ulteriori informazioni, vedere [controllare la messaggistica esterna in una rete di Yammer con le regole di trasporto di Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="24d64-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

