---
title: Configurare Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657933"
---
# <a name="configure-endpoint-dlp"></a>Configurare Endpoint DLP

Microsoft Endpoint DLP consente di rafforzare la protezione e il controllo per la prevenzione della perdita dei dati sensibili sui dispositivi Windows 10. Una volta completato l'onboarding dei dispositivi in Gestione dispositivi, è possibile creare criteri di prevenzione della perdita dei dati per applicare azioni di protezione per gli elementi. Esplora attività può essere usato per monitorare le attività per gli elementi sensibili. Per altre informazioni, vedere [Onboarding di dispositivi nella gestione dei dispositivi](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Per iniziare a usare Endpoint DLP:

- Verificare di avere la licenza per SKU/abbonamenti appropriata. Per altre informazioni, vedere [Licenze per SKU/abbonamenti](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Verificare le autorizzazioni necessarie per abilitare la gestione dei dispositivi, accedere alla pagina di onboarding, o attivare o disattivare il controllo dei dispositivi. Per altre informazioni, vedere [Autorizzazioni](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Eseguire l'onboarding dei dispositivi in Gestione dispositivi seguendo la procedura di onboarding dei dispositivi. Per altre informazioni, vedere [Onboarding di dispositivi](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Creare i criteri di prevenzione della perdita dei dati per proteggere gli elementi sensibili. Per altre informazioni, vedere [Scenari dei criteri di Endpoint DLP](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Per altre informazioni su Microsoft Endpoint DLP, veder [Informazioni sulla prevenzione della perdita di dati degli endpoint di Microsoft 365 (anteprima)](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Passaggi importanti per la raccolta dei dati, se serve assistenza:**

1. Scaricare [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. Eseguire lo strumento come amministratore dalla finestra di comando:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Quando viene richiesto, **Immettere il numero di minuti per raccogliere le tracce:**, immettere il numero di minuti necessari per eseguire lo scenario.
1. Eseguire lo scenario.

Raccogliere l'output del file ZIP da fornire all'agente di supporto.
