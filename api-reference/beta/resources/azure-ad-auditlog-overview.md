---
title: Übersicht über die Überwachungsprotokoll-API in Azure AD
description: Azure Active Directory (Azure AD) verfolgt Benutzeraktivitäten und Anmeldemetriken und erstellt Überwachungsprotokollberichte, mit deren Hilfe Sie verstehen können, wie Ihre Benutzer auf Azure AD-Dienste zugreifen und diese nutzen. Verwenden Sie die Microsoft Graph-API für Azure AD, um die Daten zu analysieren, die diesen Berichten zugrunde liegen, und um benutzerdefinierte Lösungen zu erstellen, die den speziellen Anforderungen Ihrer Organisation entsprechen.
localization_priority: Priority
ms.openlocfilehash: 89be0007ae6c13fb48ba165ca991f5dfa9d9b9cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509602"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="d88a7-104">Übersicht über die Überwachungsprotokoll-API in Azure AD</span><span class="sxs-lookup"><span data-stu-id="d88a7-104">Azure AD audit log API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d88a7-105">Azure Active Directory (Azure AD) verfolgt Benutzeraktivitäten und Anmeldemetriken und erstellt Überwachungsprotokollberichte, mit deren Hilfe Sie verstehen können, wie Ihre Benutzer auf Azure AD-Dienste zugreifen und diese nutzen.</span><span class="sxs-lookup"><span data-stu-id="d88a7-105">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and leverage Azure AD services.</span></span> <span data-ttu-id="d88a7-106">Verwenden Sie die Microsoft Graph-API für Azure AD, um die Daten zu analysieren, die diesen Berichten zugrunde liegen, und um benutzerdefinierte Lösungen zu erstellen, die den speziellen Anforderungen Ihrer Organisation entsprechen.</span><span class="sxs-lookup"><span data-stu-id="d88a7-106">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="d88a7-107">Was sind Azure AD-Aktivitätsprotokolle?</span><span class="sxs-lookup"><span data-stu-id="d88a7-107">What are Azure AD activity logs?</span></span>

<span data-ttu-id="d88a7-108">Azure AD bietet zwei Arten von Aktivitätsprotokollen:</span><span class="sxs-lookup"><span data-stu-id="d88a7-108">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="d88a7-109">Überwachungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="d88a7-109">audit logs</span></span> 
- <span data-ttu-id="d88a7-110">Anmeldeprotokolle</span><span class="sxs-lookup"><span data-stu-id="d88a7-110">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="d88a7-111">Überwachungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="d88a7-111">Audit logs</span></span>

<span data-ttu-id="d88a7-112">Der Aktivitätsbericht mit Überwachungsprotokollen bietet Ihnen Zugriff auf den Verlauf jeder einzelnen Aufgabe, die in Ihrem Mandanten ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="d88a7-112">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="d88a7-113">Der Überwachungsprotokollbericht enthält zur Compliance Datensätze mit Systemaktivitäten.</span><span class="sxs-lookup"><span data-stu-id="d88a7-113">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="d88a7-114">Die bereitgestellten Daten können Sie u. a. in den folgenden häufigen Szenarien verwenden:</span><span class="sxs-lookup"><span data-stu-id="d88a7-114">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="d88a7-115">Wer hat einem Verzeichnisbenutzer Administratorgruppenzugriff gewährt?</span><span class="sxs-lookup"><span data-stu-id="d88a7-115">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="d88a7-116">Welche Benutzer melden sich bei einer kürzlich erworbenen App an?</span><span class="sxs-lookup"><span data-stu-id="d88a7-116">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="d88a7-117">Wie viele Kennwortzurücksetzungen wurden im Verzeichnis vorgenommen?</span><span class="sxs-lookup"><span data-stu-id="d88a7-117">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="d88a7-118">Anmeldeprotokolle</span><span class="sxs-lookup"><span data-stu-id="d88a7-118">Sign in logs</span></span>

<span data-ttu-id="d88a7-119">Anhand des Aktivitätsberichts mit Anmeldeprotokollen können Sie ermitteln, wer die in den Überwachungsprotokollberichten gemeldeten Aufgaben ausgeführt hat.</span><span class="sxs-lookup"><span data-stu-id="d88a7-119">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="d88a7-120">Mit dem Aktivitätsbericht mit Anmeldungen können Sie folgende Fragen beantworten:</span><span class="sxs-lookup"><span data-stu-id="d88a7-120">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="d88a7-121">Wie sieht das Anmeldemuster eines Benutzers aus?</span><span class="sxs-lookup"><span data-stu-id="d88a7-121">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="d88a7-122">Wie viele Benutzer haben sich in der letzten Woche angemeldet?</span><span class="sxs-lookup"><span data-stu-id="d88a7-122">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="d88a7-123">Was ist der Status dieser Anmeldungen?</span><span class="sxs-lookup"><span data-stu-id="d88a7-123">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="d88a7-124">Wozu kann ich Überwachungsprotokoll-APIs in Microsoft Graph verwenden?</span><span class="sxs-lookup"><span data-stu-id="d88a7-124">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="d88a7-125">Nachfolgend finden Sie häufige Anfragen zum Arbeiten mit Überwachungsprotokolldaten:</span><span class="sxs-lookup"><span data-stu-id="d88a7-125">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="d88a7-126">Vorgang</span><span class="sxs-lookup"><span data-stu-id="d88a7-126">Operation</span></span> | <span data-ttu-id="d88a7-127">URL</span><span class="sxs-lookup"><span data-stu-id="d88a7-127">URL</span></span>
:----------|:----
<span data-ttu-id="d88a7-128">Benutzeraktivitäten des Mandanten abrufen</span><span class="sxs-lookup"><span data-stu-id="d88a7-128">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="d88a7-129">Benutzeranmeldungen des Mandanten abrufen</span><span class="sxs-lookup"><span data-stu-id="d88a7-129">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="d88a7-130">Welche Lizenzen benötige ich?</span><span class="sxs-lookup"><span data-stu-id="d88a7-130">What licenses do I need?</span></span>

<span data-ttu-id="d88a7-131">Überwachungsprotokollberichte stehen für Features zur Verfügung, die Sie lizenziert haben.</span><span class="sxs-lookup"><span data-stu-id="d88a7-131">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="d88a7-132">Wenn Sie über eine Lizenz für ein bestimmtes Feature verfügen, haben Sie auch Zugriff auf seine Überwachungsprotokolle.</span><span class="sxs-lookup"><span data-stu-id="d88a7-132">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="d88a7-133">Sie benötigen beispielsweise eine P1-Lizenz für Azure AD Premium, um auf die Self-Service-Kennwortüberwachungsberichte zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="d88a7-133">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="d88a7-134">Weitere Informationen finden Sie unter [Azure AD-Lizenzierung](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="d88a7-134">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="d88a7-135">Für Anmeldeberichte ist eine Azure AD Premium-Lizenz erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d88a7-135">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="d88a7-136">Weitere Informationen finden Sie unter [Azure AD – Preise](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="d88a7-136">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="d88a7-137">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="d88a7-137">Next Steps</span></span>

- <span data-ttu-id="d88a7-138">[Registrieren Sie Ihre App](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal), um die Voraussetzungen für Überwachungsprotokolle zu erfüllen.</span><span class="sxs-lookup"><span data-stu-id="d88a7-138">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="d88a7-139">Sehen Sie sich die Beispiele für [Überwachungsprotokolle](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) und [Anmeldeprotokolle](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples) an.</span><span class="sxs-lookup"><span data-stu-id="d88a7-139">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="d88a7-140">Überprüfen Sie die [directoryAudit](directoryaudit.md)-Ressourcen und -Aktionen.</span><span class="sxs-lookup"><span data-stu-id="d88a7-140">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="d88a7-141">Überprüfen Sie die [signIn](signin.md)-Ressourcen und -Aktionen.</span><span class="sxs-lookup"><span data-stu-id="d88a7-141">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
