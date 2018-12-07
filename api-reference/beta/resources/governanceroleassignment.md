---
title: Ressourcentyp governanceRoleAssignment
description: Stellt die Zuordnung eines Benutzers oder einer Gruppe zu einer Rolle dar.
ms.openlocfilehash: 3b0520f4641c961358b2db990914fbdf8de254f8
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191137"
---
# <a name="governanceroleassignment-resource-type"></a>Ressourcentyp governanceRoleAssignment
> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Zuordnung eines Benutzers oder einer Gruppe zu einer Rolle dar.

Privilegierten Identity Management (PIM) unterstützt zwei Arten von Zuordnungen:

1. Aktive Zuweisung - werden den Direct/aktiviert Zugriff auf Ressourcen darstellt.
2. Berechtigte Assignment - stellt eine Zwischenstufe Systemzugriff zu Ressourcen, zwischen keine Access und den direkten Zugriff. Administratoren können Benutzer/Gruppen zu zuweisen `eligible assignment` im voraus, und wenn der Zugriff benötigt, `activation` auf die `eligible assignment` ist erforderlich, um den direkten Zugriff auf die Ressource für mehrere Stunden zu erhalten. Nach der Aktivierung ein `active assignment` für die Benutzer-Gruppe Mitglieder an, dass der aktivierte Status erstellt werden.

## <a name="methods"></a>Methoden

| Methode          | Rückgabetyp |Beschreibung|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |Lesen Sie Eigenschaften und Beziehungen einer Rolle Zuordnung Entität.|
|[List](../api/governanceroleassignment-list.md) | [GovernanceRoleAssignment](../resources/governanceroleassignment.md) -Auflistung|Eine Auflistung von rollenzuweisungen für eine Ressource aufgelistet. |
|[Export](../api/governanceroleassignment-export.md) | Oktett-stream |Laden Sie eine Auflistung von rollenzuweisungen für eine Ressource, und speichern Sie als eine `.csv` Datei.|

Nicht `POST`, `PUT`, `PATCH`, oder `DELETE` Vorgänge werden unterstützt, auf die `roleAssignments` Entität festlegen. Alle erstellen, aktualisieren und Löschen von Vorgängen auf `governanceRoleAssignment` erfolgen durch `governanceRoleAssignmentRequest`.

## <a name="properties"></a>Eigenschaften
| Eigenschaft  | Typ      |Beschreibung|
|:----------|:----------|:----------|
|id         |String     |Die ID der rollenzuweisung. Es ist im GUID-Format.|
|resourceId |Zeichenfolge     |Erforderlich. Die ID der Ressource dem rollenzuweisung zugeordnet ist. |
|roleDefinitionId|Zeichenfolge|Erforderlich. Die ID der Rollendefinition dem rollenzuweisung zugeordnet ist. |
|subjectId|Zeichenfolge       |Erforderlich. Die ID des Betreffs, dem die rollenzuweisung zugeordnet ist. |
|linkedEligibleRoleAssignmentId|String|Ist dies ein `active assignment` und aufgrund der Aktivierung auf erstellt eine `eligible assignment`, es stellt die ID des, `eligible assignment`; Andernfalls ist der Wert `null`. |
|externalId   |String     |Die externe ID der Ressource, die verwendet wird, um die rollenzuweisung im Anbieter zu identifizieren.|
|startDateTime|DateTimeOffset|Die Anfangszeit der rollenzuweisung. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|Für eine vorübergehende rollenzuweisung ist dies die Uhrzeit, wann die rollenzuweisung abgelaufen ist. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|assignmentState|String  |Der Status der Zuordnung. Der Wert kann sein <ul><li> `Eligible`für die Zuweisung von zu auswählbaren</li><li> `Active`-Wenn sie direkt zugeordnet ist `Active` von Administratoren, oder bei einer Zuordnung zu auswählbaren durch den Benutzer aktiviert.</li></ul>|
|memberType|String      |Der Typ des Elements. Der Wert kann sein: <ul><li>`Inherited`-die rollenzuweisung wird von einer übergeordneten Ressourcenbereich geerbt</li><li>`Group`-die rollenzuweisung nicht geerbt wird, aber die Mitgliedschaft in einer Gruppe zuweisen stammt</li><li>`User`-die rollenzuweisung wird weder geerbt noch aus einer Gruppe zuweisen.</li></ul>|


## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Schreibgeschützt. Die Ressource, die rollenzuweisung zugeordnet. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Schreibgeschützt. Die Rollendefinition mit der rollenzuweisung verknüpft ist. |
|Betreff|[governanceSubject](../resources/governancesubject.md)|Schreibgeschützt. Der Betreff der Zuordnung Rolle zugeordnet ist. |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Schreibgeschützt. Ist dies ein `active assignment` und aufgrund der Aktivierung auf erstellt eine `eligible assignment`, es stellt das Objekt, das `eligible assignment`; Andernfalls ist der Wert `null`. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
