---
title: Azure AD Audit Log-API (Übersicht)
description: Azure Active Directory (AD Azure) Benutzer Aktivität und Anmeldung Metriken verfolgt und erstellt Audit Log-Berichte, die Ihnen helfen zu verstehen, wie Ihre Benutzer zugreifen und Azure AD-Dienste nutzen. Verwenden Sie die Microsoft Graph-API für Azure AD, um die zugrunde liegenden dieser Berichte Daten zu analysieren und zum Erstellen benutzerdefinierter Lösungen, die auf bestimmte Anforderungen Ihrer Organisation zugeschnitten.
ms.openlocfilehash: b25e9820d4f6df0c6a38fc9784a37ce8a82ceeb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059592"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="faba2-104">Azure AD Audit Log-API (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="faba2-104">Azure AD audit log API overview</span></span>

> <span data-ttu-id="faba2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="faba2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faba2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="faba2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="faba2-107">Azure Active Directory (AD Azure) Benutzer Aktivität und Anmeldung Metriken verfolgt und erstellt Audit Log-Berichte, die Ihnen helfen zu verstehen, wie Ihre Benutzer zugreifen und Azure AD-Dienste nutzen.</span><span class="sxs-lookup"><span data-stu-id="faba2-107">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and leverage Azure AD services.</span></span> <span data-ttu-id="faba2-108">Verwenden Sie die Microsoft Graph-API für Azure AD, um die zugrunde liegenden dieser Berichte Daten zu analysieren und zum Erstellen benutzerdefinierter Lösungen, die auf bestimmte Anforderungen Ihrer Organisation zugeschnitten.</span><span class="sxs-lookup"><span data-stu-id="faba2-108">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="faba2-109">Was sind Azure AD-Aktivität protokolliert?</span><span class="sxs-lookup"><span data-stu-id="faba2-109">What are Azure AD activity logs?</span></span>

<span data-ttu-id="faba2-110">Azure AD bietet zwei Arten von Aktivitätsprotokolle:</span><span class="sxs-lookup"><span data-stu-id="faba2-110">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="faba2-111">Überwachungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="faba2-111">audit logs</span></span> 
- <span data-ttu-id="faba2-112">-in-Protokolle</span><span class="sxs-lookup"><span data-stu-id="faba2-112">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="faba2-113">Überwachungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="faba2-113">Audit logs</span></span>

<span data-ttu-id="faba2-114">Die Protokolle Aktivität Überwachungsbericht bietet Zugriff auf den Verlauf jeder Aufgabe, die in Ihrem Mandanten ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="faba2-114">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="faba2-115">Die Protokolle Überwachungsbericht enthält Datensätze für die Einhaltung der Systemaktivitäten.</span><span class="sxs-lookup"><span data-stu-id="faba2-115">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="faba2-116">Unter anderem können bereitgestellten Daten Sie gängige Szenarien wie behandeln:</span><span class="sxs-lookup"><span data-stu-id="faba2-116">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="faba2-117">Die einem Benutzer Directory Gruppe Administratorzugriff gewährt?</span><span class="sxs-lookup"><span data-stu-id="faba2-117">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="faba2-118">Welche Benutzer zu einer kürzlich erworbenen app anmelden?</span><span class="sxs-lookup"><span data-stu-id="faba2-118">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="faba2-119">Wie viele Kennwörter zurückgesetzt wurden in das Verzeichnis vorgenommen?</span><span class="sxs-lookup"><span data-stu-id="faba2-119">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="faba2-120">Melden Sie sich die Protokolle</span><span class="sxs-lookup"><span data-stu-id="faba2-120">Sign in logs</span></span>

<span data-ttu-id="faba2-121">Der Aktivitätsbericht Anmeldungen können Sie bestimmen, wer die berichtet von Überwachungsprotokollberichte Aufgaben durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="faba2-121">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="faba2-122">Der Bericht über Benutzeraktivität Anmeldungen hilft Ihnen Fragen beantworten:</span><span class="sxs-lookup"><span data-stu-id="faba2-122">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="faba2-123">Was ist das Zeichen in Muster eines Benutzers?</span><span class="sxs-lookup"><span data-stu-id="faba2-123">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="faba2-124">Wie viele Benutzer während der letzten Woche angemeldet haben?</span><span class="sxs-lookup"><span data-stu-id="faba2-124">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="faba2-125">Was ist der Status der diese Anmeldungen?</span><span class="sxs-lookup"><span data-stu-id="faba2-125">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="faba2-126">Was kann ich mit Überwachungsprotokoll-APIs in Microsoft Graph machen?</span><span class="sxs-lookup"><span data-stu-id="faba2-126">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="faba2-127">Es folgen beliebte Anforderungen für die Arbeit mit Audit Log-Daten:</span><span class="sxs-lookup"><span data-stu-id="faba2-127">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="faba2-128">Vorgang</span><span class="sxs-lookup"><span data-stu-id="faba2-128">Operation</span></span> | <span data-ttu-id="faba2-129">URL</span><span class="sxs-lookup"><span data-stu-id="faba2-129">URL</span></span>
:----------|:----
<span data-ttu-id="faba2-130">Abrufen von Mandanten die Benutzeraktivitäten</span><span class="sxs-lookup"><span data-stu-id="faba2-130">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="faba2-131">Abrufen von Mandanten benutzeranmeldungen</span><span class="sxs-lookup"><span data-stu-id="faba2-131">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="faba2-132">Welche Lizenzen benötige ich?</span><span class="sxs-lookup"><span data-stu-id="faba2-132">What licenses do I need?</span></span>

<span data-ttu-id="faba2-133">Überwachungsprotokollberichte stehen für Features, die Sie lizenziert haben.</span><span class="sxs-lookup"><span data-stu-id="faba2-133">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="faba2-134">Wenn Sie eine Lizenz für ein bestimmtes Feature verfügen, haben Sie auch Zugriff auf die Überwachungsprotokolle.</span><span class="sxs-lookup"><span data-stu-id="faba2-134">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="faba2-135">Beispielsweise benötigen Sie eine Azure AD Premium P1-Lizenz auf Self-service Password Überwachungsberichte zugreifen.</span><span class="sxs-lookup"><span data-stu-id="faba2-135">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="faba2-136">Finden Sie weitere Informationen finden Sie unter [Azure AD-Lizenzierung](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="faba2-136">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="faba2-137">-In Reports ist eine Azure AD Premium-Lizenz erforderlich.</span><span class="sxs-lookup"><span data-stu-id="faba2-137">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="faba2-138">Finden Sie weitere Informationen finden Sie unter [Preise Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="faba2-138">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="faba2-139">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="faba2-139">Next Steps</span></span>

- <span data-ttu-id="faba2-140">[Registrieren Sie Ihre app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) , um Audit Log Voraussetzungen erfüllen.</span><span class="sxs-lookup"><span data-stu-id="faba2-140">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="faba2-141">Lernen Sie [Überwachungsprotokoll](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) und [Anmeldung Beispiele](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="faba2-141">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="faba2-142">Die [DirectoryAudit](directoryaudit.md) Ressource überprüfen und Aktionen.</span><span class="sxs-lookup"><span data-stu-id="faba2-142">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="faba2-143">Die [Anmeldung](signin.md) Ressource überprüfen und Aktionen.</span><span class="sxs-lookup"><span data-stu-id="faba2-143">Review [signIn](signin.md) resource and actions.</span></span> 