---
title: Ressourcentyp privilegedRoleAssignmentRequest
description: Stellt die Anforderung für Role Assignment Vorgänge in Privilegd Identity Management.
localization_priority: Normal
ms.openlocfilehash: c0e0bbfa76b7ffb4e122d381d45dd4092f0843c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509007"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a>Ressourcentyp privilegedRoleAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die Anforderung für Role Assignment Vorgänge in Privilegd Identity Management.

`privilegedRoleAssignmentRequest`wird eine Entität Ticket modelliert verwaltet den Lebenszyklus von rollenzuweisungen. Es stellt die Absicht/Entscheidung von Benutzern und Administratoren und bietet außerdem die Flexibilität zum Aktivieren der Implementierung von wiederkehrenden Schduling, Gates Genehmigung und usw., im Vergleich zu direkt Verfügbarmachen `POST` und `LIST` Vorgänge sowie `MY` und `Cancel` -Funktionen auf `governanceRoleAssignment`.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp | Beschreibung |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | [Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) -Auflistung|Role Assignment Anforderungen aufgelistet.|
|[Create](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Erstellen Sie eine Anforderung an den Lebenszyklus von vorhandenen oder neuen rollenzuweisung zu verwalten.|
|[Cancel](../api/privilegedroleassignmentrequest-cancel.md)|  |Ausstehende Role Assignment Anforderung abbrechen.|
|[My](../api/privilegedroleassignmentrequest-my.md)|  |GET-Anforderung für Rolle-Zuordnung für aktuellen Requstor.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|id|String| Schreibgeschützt. Die Id der Rolle Zuordnung Anforderung.|
|assignmentState|String| Der Status der Zuordnung. Der Wert kann sein `Eligible` für die Zuweisung von zu auswählbaren `Active` – Wenn sie direkt zugeordnet ist `Active` von Administratoren, oder an einer Zuordnung zu auswählbaren durch den Benutzer aktiviert.|
|duration|String| Die Dauer einer rollenzuweisung.|
|Grund|String| Der Grund für die rollenzuweisung.|
|requestedDateTime|DateTimeOffset| Schreibgeschützt. Die Zeit zu erstellen. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|roleId|String| Die Id der Rolle.|
|Zeitplan|[governanceSchedule](governanceschedule.md)| Das der Rolle Zuordnung Anforderung Zeitplan-Objekt.|
|status|Zeichenfolge| Lesen vorbehalten Status der Anforderung Zuordnung Rolle. Der Wert kann sein `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.|
|ticketNumber|String| Die TicketNumber für die rollenzuweisung. |
|ticketSystem|String| Die TicketSystem für die rollenzuweisung.|
|type|String| Darstellen der den Typ des Vorgangs für die rollenzuweisung. Der Wert kann sein `AdminAdd`: Administratoren hinzufügen von Benutzern zu Rollen; `UserAdd`: Hinzufügen von Benutzern rollenzuweisungen.|
|userId|String| Die Id des Benutzers.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|roleInfo|[privilegedRole](privilegedrole.md)| Das Objekt RoleInfo der Rolle Zuordnung Anforderung.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
}-->

```json
{
  "assignmentState": "String",
  "duration": "String",
  "id": "String (identifier)",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "roleId": "String",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": "String",
  "ticketNumber": "String",
  "ticketSystem": "String",
  "type": "String",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
