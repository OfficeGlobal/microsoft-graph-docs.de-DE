---
title: appRoleAssignment-Ressourcentyp
description: Dient zum Aufzeichnen, wann ein Benutzer oder eine Gruppe einer Anwendung zugewiesen wird. In diesem Fall führt die Rollenzuweisung dazu, dass die Anwendungskachel im App-Zugriffsbereich des Benutzers angezeigt wird. Diese Entität kann auch verwendet werden, um einer anderen Anwendung (als Dienstprinzipal modelliert) Zugriff auf eine Ressourcenanwendung in einer bestimmten Rolle zu gewähren. Sie können Rollenzuweisungen erstellen, lesen, aktualisieren und löschen.
localization_priority: Priority
ms.openlocfilehash: 4e4bb6e2c9f94780dba642167ecdb9200849038f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576619"
---
# <a name="approleassignment-resource-type"></a>appRoleAssignment-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Dient zum Aufzeichnen, wann ein Benutzer oder eine Gruppe einer Anwendung zugewiesen wird. In diesem Fall führt die Rollenzuweisung dazu, dass die Anwendungskachel im App-Zugriffsbereich des Benutzers angezeigt wird. Diese Entität kann auch verwendet werden, um einer anderen Anwendung (als Dienstprinzipal modelliert) Zugriff auf eine Ressourcenanwendung in einer bestimmten Rolle zu gewähren. Sie können Rollenzuweisungen erstellen, lesen, aktualisieren und löschen.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|creationTimestamp|DateTimeOffset|Der Zeitpunkt, zu dem der Kontakt erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen:  Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|id|Guid|Die Rollen-ID, die dem Prinzipal zugewiesen wurde.  Diese Rolle muss von der Zielressourcenanwendung **ResourceId** in der **appRoles**-Eigenschaft deklariert werden. Wenn die Ressource keine Berechtigungen deklariert, muss eine Standard-ID (GUID von 0) angegeben werden. Schlüssel. Nullwerte zulassend. |
|principalDisplayName|Zeichenfolge|Der Anzeigename des Prinzipals, dem Zugriff gewährt wurde.|
|principalId|Guid|Der eindeutige Bezeichner (**Id**) für den Prinzipal, dem Zugriff gewährt wird. Beim Erstellen erforderlich.            |
|principalType|Zeichenfolge|Der Prinzipaltyp.  Dies kann entweder „Benutzer“, „Gruppe“ oder „ServicePrincipal“ sein.|
|resourceDisplayName|Zeichenfolge|Der Anzeigename der Ressource, für die die Zuweisung erfolgte.|
|resourceId|Guid|Die eindeutige ID (**Id**) für die Zielressource (Dienstprinzipal), für die die Zuweisung vorgenommen wurde.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[appRoleAssignment abrufen](../api/approleassignment-get.md) | [appRoleAssignment](approleassignment.md) |Lesen von Eigenschaften und Beziehungen des approleAssignment-Objekts.|
|[Update](../api/approleassignment-update.md) | [appRoleAssignment](approleassignment.md)   |Aktualisieren des approleassignment-Objekts. |
|[Delete](../api/approleassignment-delete.md) | Keine |Löschen des approleassignment-Objekts. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
