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
# <a name="azure-ad-audit-log-api-overview"></a>Übersicht über die Überwachungsprotokoll-API in Azure AD

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) verfolgt Benutzeraktivitäten und Anmeldemetriken und erstellt Überwachungsprotokollberichte, mit deren Hilfe Sie verstehen können, wie Ihre Benutzer auf Azure AD-Dienste zugreifen und diese nutzen. Verwenden Sie die Microsoft Graph-API für Azure AD, um die Daten zu analysieren, die diesen Berichten zugrunde liegen, und um benutzerdefinierte Lösungen zu erstellen, die den speziellen Anforderungen Ihrer Organisation entsprechen.

## <a name="what-are-azure-ad-activity-logs"></a>Was sind Azure AD-Aktivitätsprotokolle?

Azure AD bietet zwei Arten von Aktivitätsprotokollen:

- Überwachungsprotokolle 
- Anmeldeprotokolle

### <a name="audit-logs"></a>Überwachungsprotokolle

Der Aktivitätsbericht mit Überwachungsprotokollen bietet Ihnen Zugriff auf den Verlauf jeder einzelnen Aufgabe, die in Ihrem Mandanten ausgeführt wurde. Der Überwachungsprotokollbericht enthält zur Compliance Datensätze mit Systemaktivitäten. Die bereitgestellten Daten können Sie u. a. in den folgenden häufigen Szenarien verwenden:

- Wer hat einem Verzeichnisbenutzer Administratorgruppenzugriff gewährt?

- Welche Benutzer melden sich bei einer kürzlich erworbenen App an?

- Wie viele Kennwortzurücksetzungen wurden im Verzeichnis vorgenommen?

### <a name="sign-in-logs"></a>Anmeldeprotokolle

Anhand des Aktivitätsberichts mit Anmeldeprotokollen können Sie ermitteln, wer die in den Überwachungsprotokollberichten gemeldeten Aufgaben ausgeführt hat. Mit dem Aktivitätsbericht mit Anmeldungen können Sie folgende Fragen beantworten:

- Wie sieht das Anmeldemuster eines Benutzers aus?
- Wie viele Benutzer haben sich in der letzten Woche angemeldet?
- Was ist der Status dieser Anmeldungen?

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>Wozu kann ich Überwachungsprotokoll-APIs in Microsoft Graph verwenden?

Nachfolgend finden Sie häufige Anfragen zum Arbeiten mit Überwachungsprotokolldaten:

Vorgang | URL
:----------|:----
Benutzeraktivitäten des Mandanten abrufen | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
Benutzeranmeldungen des Mandanten abrufen | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a>Welche Lizenzen benötige ich?

Überwachungsprotokollberichte stehen für Features zur Verfügung, die Sie lizenziert haben.  Wenn Sie über eine Lizenz für ein bestimmtes Feature verfügen, haben Sie auch Zugriff auf seine Überwachungsprotokolle.

Sie benötigen beispielsweise eine P1-Lizenz für Azure AD Premium, um auf die Self-Service-Kennwortüberwachungsberichte zuzugreifen.  Weitere Informationen finden Sie unter [Azure AD-Lizenzierung](https://azure.microsoft.com/pricing/details/active-directory/).

Für Anmeldeberichte ist eine Azure AD Premium-Lizenz erforderlich.

Weitere Informationen finden Sie unter [Azure AD – Preise](https://azure.microsoft.com/pricing/details/active-directory/).

## <a name="next-steps"></a>Nächste Schritte

- [Registrieren Sie Ihre App](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal), um die Voraussetzungen für Überwachungsprotokolle zu erfüllen. 
- Sehen Sie sich die Beispiele für [Überwachungsprotokolle](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) und [Anmeldeprotokolle](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples) an.  
- Überprüfen Sie die [directoryAudit](directoryaudit.md)-Ressourcen und -Aktionen.
- Überprüfen Sie die [signIn](signin.md)-Ressourcen und -Aktionen. 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
