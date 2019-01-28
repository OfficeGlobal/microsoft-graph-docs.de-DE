---
title: Verwenden der Benachrichtigungs-REST-API in Microsoft Graph
description: Sie können die Benachrichtigungs-API in Microsoft Graph verwenden, um Pushbenachrichtigungen an einen Benutzer zu senden. Wählen Sie einfach ein Benutzerkonto aus, an das eine Benachrichtigung gesendet werden soll; die Plattform übermittelt die Benachrichtigung dann an alle Geräteendpunkte. Benachrichtigungs-API-Anfragen werden im Auftrag eines Benutzers über delegierte Berechtigungen und die [Benachrichtigungsberechtigung]( /graph/permissions_reference) ausgeführt, die mit Microsoft-Konten oder mit Geschäfts-oder Schulkonten verwendet werden können.
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 2a4c23955e348159d2e17514d6041260f13cffba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513984"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Verwenden der Benachrichtigungs-REST-API in Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können die Benachrichtigungs-API in Microsoft Graph verwenden, um Pushbenachrichtigungen an einen Benutzer zu senden. Wählen Sie einfach ein Benutzerkonto aus, an das eine Benachrichtigung gesendet werden soll; die Plattform übermittelt die Benachrichtigung dann an alle Geräteendpunkte. Benachrichtigungs-API-Anfragen werden im Auftrag eines Benutzers über [delegierte Berechtigungen](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) und die [Benachrichtigungsberechtigung]( /graph/permissions_reference) ausgeführt, die mit Microsoft-Konten oder mit Geschäfts-oder Schulkonten verwendet werden können.
Diese Art von benutzerzentrierter Benachrichtigung wird von der [notification](../resources/projectrome-notification.md)-Ressource dargestellt und wird in Microsoft Graph gespeichert. Diese kann dann von der Veröffentlichungs-App über die [Project Rome-SDK-APIs](https://github.com/Microsoft/project-rome) geöffnet und verwaltet werden. 

## <a name="next-steps"></a>Nächste Schritte
- Sehen Sie sich die [notification-Ressource](../resources/projectrome-notification.md) an, und erstellen Sie Benachrichtigungen, um mit Ihren Benutzern zu interagieren. 
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/notifications-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
