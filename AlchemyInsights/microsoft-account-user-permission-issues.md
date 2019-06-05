---
title: Creare e utilizzare una cassetta postale condivisa
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717351"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="e80ab-102">Risoluzione dei problemi relativi a un utente non trovato nella directory</span><span class="sxs-lookup"><span data-stu-id="e80ab-102">Troubleshoot issue - User not found in directory</span></span>

<p><span data-ttu-id="e80ab-103">Se gli utenti ricevono un messaggio <strong> &ldquo; &hellip;di errore&rsquo;, l'utente non può essere trovato nella directory. Provare di nuovo&hellip; </strong> in cui il tipo di problema è <strong> &ldquo;utente non presente&rdquo;nella directory.</strong>, è possibile completare i passaggi seguenti per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="e80ab-103">If users are receiving error message <strong>&ldquo;&hellip;user can&rsquo;t be found in the directory. Please try again&hellip;&rdquo;</strong> where the Issue Type is <strong>&ldquo;User not in directory.&rdquo;</strong>, the following steps can be completed to troubleshoot the issue.</span></span></p> <ol> <li><span data-ttu-id="e80ab-104">Verificare che l'account che ha accettato l'invito alla posta elettronica sia lo stesso utilizzato per l'accesso in un secondo momento.</span><span class="sxs-lookup"><span data-stu-id="e80ab-104">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="e80ab-105">Assicurarsi che l'utente stia utilizzando lo stesso account per accettare l'invito e accedere al sito.</span><span class="sxs-lookup"><span data-stu-id="e80ab-105">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> <br /><br /><span data-ttu-id="e80ab-106">Per altre informazioni, vedere <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">How to Manage aliases for your Microsoft account</a> to manage the Office 365 login.</span><span class="sxs-lookup"><span data-stu-id="e80ab-106">For more info, see <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">How to manage aliases for your Microsoft account</a> to manage the Office 365 login.</span></span> <br /><br /></li> <li><span data-ttu-id="e80ab-107">Passare a ogni sito o i siti in cui l'utente riceve l'errore.</span><span class="sxs-lookup"><span data-stu-id="e80ab-107">Browse to each site(s) in which the user is receiving the error.</span></span> <br /><br /><span data-ttu-id="e80ab-108">un.</span><span class="sxs-lookup"><span data-stu-id="e80ab-108">a.</span></span> <span data-ttu-id="e80ab-109">Aggiungere <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid = 0&rdquo; </strong> (tra virgolette doppie) alla fine dell'URL del sito.</span><span class="sxs-lookup"><span data-stu-id="e80ab-109">Add <strong>&ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo;</strong> (within the double-quotes) to the end of the site URL.</span></span> <br /><br /><span data-ttu-id="e80ab-110">Esempio: https://&lt;contoso&gt;. SharePoint.com/_layouts/15/people.aspx/membershipGroupId=0</span><span class="sxs-lookup"><span data-stu-id="e80ab-110">Example: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0</span></span> <br /><br /><span data-ttu-id="e80ab-111">b.</span><span class="sxs-lookup"><span data-stu-id="e80ab-111">b.</span></span> <span data-ttu-id="e80ab-112">Selezionare l'utente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="e80ab-112">Select the user from the list.</span></span> <br /><br /><span data-ttu-id="e80ab-113">c.</span><span class="sxs-lookup"><span data-stu-id="e80ab-113">c.</span></span> <span data-ttu-id="e80ab-114">Fare clic su <strong>Rimuovi autorizzazioni utente dalla barra multifunzione</strong>.</span><span class="sxs-lookup"><span data-stu-id="e80ab-114">Click <strong>Remove User Permissions from the Ribbon</strong>.</span></span> <br /><br /><span data-ttu-id="e80ab-115">d.</span><span class="sxs-lookup"><span data-stu-id="e80ab-115">d.</span></span> <span data-ttu-id="e80ab-116">Aggiungere di nuovo l'utente e rinviare l'invito all'utente.</span><span class="sxs-lookup"><span data-stu-id="e80ab-116">Add back the User and Resend the invite to the user.</span></span></li> </ol>
