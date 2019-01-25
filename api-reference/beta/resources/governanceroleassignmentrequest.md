---
title: Ressourcentyp governanceRoleAssignmentRequest
description: Stellt die Anforderung für Role Assignment Vorgänge in Privilegd Identity Management.
localization_priority: Normal
ms.openlocfilehash: 242f1d311a2d304d0d8dab0a4e24f9294722ab6e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509574"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>Ressourcentyp governanceRoleAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|id                         |Zeichenfolge         |Die Id der Rolle Zuordnung Anforderung.|
|resourceId                 |Zeichenfolge         |Erforderlich. Die Id der Ressource dem die Rolle Zuordnung Anforderung zugeordnet ist.|
|roleDefinitionId           |Zeichenfolge         |Erforderlich. Die Id der Rollendefinition, dem die Rolle Zuordnung Anforderung zugeordnet ist.|
|subjectId                  |Zeichenfolge         |Erforderlich. Die Id des Betreffs, dem die Rolle Zuordnung Anforderung zugeordnet ist.|
|type                       |String         |Erforderlich. Darstellen der den Typ des Vorgangs für die rollenzuweisung. Der Wert kann sein <ul><li>`AdminAdd`: Administratoren Benutzer/Gruppen zu Rollen zuweisen;</li><li>`UserAdd`: Benutzer aktivieren zu auswählbaren Zuordnungen;</li><li> `AdminUpdate`: Administratoren Ändern vorhandener rollenzuweisungen</li><li>`AdminRemove`: Administratoren Benutzer/Gruppen aus Rollen entfernen;<li>`UserRemove`: Benutzer deaktivieren aktive Zuordnungen;<li>`UserExtend`: Benutzer erfordern, deren ablaufenden Aufgaben zu erweitern.</li><li>`AdminExtend`: Administratoren erweitern ablaufende Zuordnungen.</li><li>`UserRenew`: Benutzer anfordern, um deren abgelaufenen Aufgaben zu erneuern.</li><li>`AdminRenew`: Administratoren erweitern ablaufende Zuordnungen.</li></ul>|
|assignmentState|Zeichenfolge  |Erforderlich. Der Status der Zuordnung. Der Wert kann sein <ul><li> `Eligible`für die Zuweisung von zu auswählbaren</li><li> `Active`-Wenn sie direkt zugeordnet ist `Active` von Administratoren, oder bei einer Zuordnung zu auswählbaren durch den Benutzer aktiviert.</li></ul>|
|requestedDateTime          |DateTimeOffset |Schreibgeschützt. Die Zeit zu erstellen. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Zeitplan                   |[governanceSchedule](governanceschedule.md)|Das der Rolle Zuordnung Anforderung Zeitplan-Objekt.|
|Grund                     |String         |Eine Nachricht stammt von Benutzern und Administratoren beim Erstellen der Anforderung zur, warum es erforderlich ist.|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |Der Status der Anforderung Zuordnung Rolle.|
|linkedEligibleRoleAssignmentId|String        |Ist dies eine Anforderung für die Aktivierung der Rolle, stellt Sie die Id des der `eligible assignment` verwiesen wird; Andernfalls ist der Wert `null`. |



## <a name="relationships"></a>Beziehungen
| Beziehung | Typ                                |Beschreibung|
|:-------------|:----------------------------------|:----------|
|resource      |[governanceResource](../resources/governanceresource.md)            |Schreibgeschützt. Die Ressource, der die Anforderung zum Ziel. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Schreibgeschützt. Die Rollendefinition, der die Anforderung zum Ziel. |
|subject       |[governanceSubject](../resources/governancesubject.md)|Schreibgeschützt. Der Prinzipal Benutzer-/Gruppen.|

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
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": {"@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"},
  "linkedEligibleRoleAssignmentId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
