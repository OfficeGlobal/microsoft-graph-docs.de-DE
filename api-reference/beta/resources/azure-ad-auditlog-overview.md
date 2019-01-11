---
title: Azure AD Audit Log-API (Übersicht)
description: Azure Active Directory (AD Azure) Benutzer Aktivität und Anmeldung Metriken verfolgt und erstellt Audit Log-Berichte, die Ihnen helfen zu verstehen, wie Ihre Benutzer zugreifen und Azure AD-Dienste nutzen. Verwenden Sie die Microsoft Graph-API für Azure AD, um die zugrunde liegenden dieser Berichte Daten zu analysieren und zum Erstellen benutzerdefinierter Lösungen, die auf bestimmte Anforderungen Ihrer Organisation zugeschnitten.
localization_priority: Priority
ms.openlocfilehash: 07d285ce4e7fbf736900c1d6d4acdf159b451424
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826222"
---
# <a name="azure-ad-audit-log-api-overview"></a>Azure AD Audit Log-API (Übersicht)

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Azure Active Directory (AD Azure) Benutzer Aktivität und Anmeldung Metriken verfolgt und erstellt Audit Log-Berichte, die Ihnen helfen zu verstehen, wie Ihre Benutzer zugreifen und Azure AD-Dienste nutzen. Verwenden Sie die Microsoft Graph-API für Azure AD, um die zugrunde liegenden dieser Berichte Daten zu analysieren und zum Erstellen benutzerdefinierter Lösungen, die auf bestimmte Anforderungen Ihrer Organisation zugeschnitten.

## <a name="what-are-azure-ad-activity-logs"></a>Was sind Azure AD-Aktivität protokolliert?

Azure AD bietet zwei Arten von Aktivitätsprotokolle:

- Überwachungsprotokolle 
- -in-Protokolle

### <a name="audit-logs"></a>Überwachungsprotokolle

Die Protokolle Aktivität Überwachungsbericht bietet Zugriff auf den Verlauf jeder Aufgabe, die in Ihrem Mandanten ausgeführt. Die Protokolle Überwachungsbericht enthält Datensätze für die Einhaltung der Systemaktivitäten. Unter anderem können bereitgestellten Daten Sie gängige Szenarien wie behandeln:

- Die einem Benutzer Directory Gruppe Administratorzugriff gewährt?

- Welche Benutzer zu einer kürzlich erworbenen app anmelden?

- Wie viele Kennwörter zurückgesetzt wurden in das Verzeichnis vorgenommen?

### <a name="sign-in-logs"></a>Melden Sie sich die Protokolle

Der Aktivitätsbericht Anmeldungen können Sie bestimmen, wer die berichtet von Überwachungsprotokollberichte Aufgaben durchgeführt. Der Bericht über Benutzeraktivität Anmeldungen hilft Ihnen Fragen beantworten:

- Was ist das Zeichen in Muster eines Benutzers?
- Wie viele Benutzer während der letzten Woche angemeldet haben?
- Was ist der Status der diese Anmeldungen?

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>Was kann ich mit Überwachungsprotokoll-APIs in Microsoft Graph machen?

Es folgen beliebte Anforderungen für die Arbeit mit Audit Log-Daten:

Vorgang | URL
:----------|:----
Abrufen von Mandanten die Benutzeraktivitäten | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
Abrufen von Mandanten benutzeranmeldungen | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a>Welche Lizenzen benötige ich?

Überwachungsprotokollberichte stehen für Features, die Sie lizenziert haben.  Wenn Sie eine Lizenz für ein bestimmtes Feature verfügen, haben Sie auch Zugriff auf die Überwachungsprotokolle.

Beispielsweise benötigen Sie eine Azure AD Premium P1-Lizenz auf Self-service Password Überwachungsberichte zugreifen.  Finden Sie weitere Informationen finden Sie unter [Azure AD-Lizenzierung](https://azure.microsoft.com/pricing/details/active-directory/).

-In Reports ist eine Azure AD Premium-Lizenz erforderlich.

Finden Sie weitere Informationen finden Sie unter [Preise Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

## <a name="next-steps"></a>Nächste Schritte

- [Registrieren Sie Ihre app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) , um Audit Log Voraussetzungen erfüllen. 
- Lernen Sie [Überwachungsprotokoll](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) und [Anmeldung Beispiele](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).  
- Die [DirectoryAudit](directoryaudit.md) Ressource überprüfen und Aktionen.
- Die [Anmeldung](signin.md) Ressource überprüfen und Aktionen. 
