---
title: Ressourcentyp governanceRoleAssignmentRequest
description: Stellt die Anforderung für Role Assignment Vorgänge in Privilegd Identity Management.
ms.openlocfilehash: 4b19ed04b4c78fa084c1247fc1798a39b08c3fdb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057944"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>Ressourcentyp governanceRoleAssignmentRequest

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Anforderung für Role Assignment Vorgänge in Privilegd Identity Management.

`governanceRoleAssignmentRequest`wird eine Entität Ticket modelliert verwaltet den Lebenszyklus von rollenzuweisungen. Es stellt die Absicht/Entscheidung von Benutzern und Administratoren und bietet außerdem die Flexibilität zum Aktivieren der Implementierung von wiederkehrenden Schduling, Gates Genehmigung und usw., im Vergleich zu direkt Verfügbarmachen `POST`, `PUT`, und `DELETE` Vorgänge Klicken Sie auf `governanceRoleAssignment`.

## <a name="methods"></a>Methoden

| Methode          |Rückgabetyp  |Beschreibung|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Abrufen einer Rolle Zuordnung Anforderung durch ID angegebenen  
|[List](../api/governanceroleassignmentrequest-list.md) | [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Auflistung|Get-Role Assignment-Anforderungen für eine Ressource.|
|[Create](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Erstellen Sie eine Anforderung an den Lebenszyklus von vorhandenen oder neuen rollenzuweisung zu verwalten.|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |Ausstehende Role Assignment Anforderung abbrechen.|
|[Update](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Administratoren aktualisieren die Entscheidung über die Anforderungen, wenn die Anforderungen in den Status der werden `PendingAdminDecision`.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft                  | Typ          |Beschreibung|
|:--------------------------|:--------------|:----------|
|id                         |String         |Die Id der Rolle Zuordnung Anforderung.|
|resourceId                 |Zeichenfolge         |Erforderlich. Die Id der Ressource dem die Rolle Zuordnung Anforderung zugeordnet ist.|
|roleDefinitionId           |Zeichenfolge         |Erforderlich. Die Id der Rollendefinition, dem die Rolle Zuordnung Anforderung zugeordnet ist.|
|subjectId                  |Zeichenfolge         |Erforderlich. Die Id des Betreffs, dem die Rolle Zuordnung Anforderung zugeordnet ist.|
|Typ                       |Zeichenfolge         |Erforderlich. Darstellen der den Typ des Vorgangs für die rollenzuweisung. Der Wert kann sein <ul><li>`AdminAdd`: Administratoren Benutzer/Gruppen zu Rollen zuweisen;</li><li>`UserAdd`: Benutzer aktivieren zu auswählbaren Zuordnungen;</li><li> `AdminUpdate`: Administratoren Ändern vorhandener rollenzuweisungen</li><li>`AdminRemove`: Administratoren Benutzer/Gruppen aus Rollen entfernen;<li>`UserRemove`: Benutzer deaktivieren aktive Zuordnungen;<li>`UserExtend`: Benutzer erfordern, deren ablaufenden Aufgaben zu erweitern.</li><li>`AdminExtend`: Administratoren erweitern ablaufende Zuordnungen.</li><li>`UserRenew`: Benutzer anfordern, um deren abgelaufenen Aufgaben zu erneuern.</li><li>`AdminRenew`: Administratoren erweitern ablaufende Zuordnungen.</li></ul>|
|assignmentState|Zeichenfolge  |Erforderlich. Der Status der Zuordnung. Der Wert kann sein <ul><li> `Eligible`für die Zuweisung von zu auswählbaren</li><li> `Active`-Wenn sie direkt zugeordnet ist `Active` von Administratoren, oder bei einer Zuordnung zu auswählbaren durch den Benutzer aktiviert.</li></ul>|
|requestedDateTime          |DateTimeOffset |Schreibgeschützt. Die Zeit zu erstellen. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|roleAssignmentStartDateTime|DateTimeOffset |Die Startzeit für die rollenzuweisung. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|roleAssignmentEndDateTime|DateTimeOffset   |Die Endzeit für die rollenzuweisung. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Zeitplan                   |[governanceSchedule](governanceschedule.md)|Das der Rolle Zuordnung Anforderung Zeitplan-Objekt.|
|Grund                     |String         |Eine Nachricht stammt von Benutzern und Administratoren beim Erstellen der Anforderung zur, warum es erforderlich ist.|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |Der Status der Anforderung Zuordnung Rolle.|
|linkedEligibleRoleAssignmentId|String        |Ist dies eine Anforderung für die Aktivierung der Rolle, stellt Sie die Id des der `eligible assignment` verwiesen wird; Andernfalls ist der Wert `null`. |



## <a name="relationships"></a>Beziehungen
| Beziehung | Typ                                |Beschreibung|
|:-------------|:----------------------------------|:----------|
|resource      |[governanceResource](../resources/governanceresource.md)            |Schreibgeschützt. Die Ressource, der die Anforderung zum Ziel. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Schreibgeschützt. Die Rollendefinition, der die Anforderung zum Ziel. |
|Betreff       |[governanceSubject](../resources/governancesubject.md)|Schreibgeschützt. Der Prinzipal Benutzer-/Gruppen.|

### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "type": "String",
  "assignmentState": "String",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "roleAssignmentStartDateTime": "String (timestamp)",
  "roleAssignmentEndDateTime": "String (timestamp)",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": {"@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"},
  "linkedEligibleRoleAssignmentId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
