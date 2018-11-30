---
title: Ressourcentyp appRoleAssignment
description: Verwendet zum Aufzeichnen, wenn ein Benutzer oder eine Gruppe zu einer Anwendung zugewiesen wird. In diesem Fall führt die rollenzuweisung Kachel Anwendung Einrichten des Benutzers app Zugriff im Bereich angezeigt. Dieser Entität kann auch verwendet werden, zu einer anderen (modelliert als Dienst principal) Anwendungszugriff auf eine Ressource-Anwendung in einer bestimmten Rolle erteilen. Sie können erstellen, lesen, aktualisieren und Löschen von rollenzuweisungen.
ms.openlocfilehash: 97155bde12735ebd8a7674e0dbf20dae30e53f14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059602"
---
# <a name="approleassignment-resource-type"></a>Ressourcentyp appRoleAssignment

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwendet zum Aufzeichnen, wenn ein Benutzer oder eine Gruppe zu einer Anwendung zugewiesen wird. In diesem Fall führt die rollenzuweisung Kachel Anwendung Einrichten des Benutzers app Zugriff im Bereich angezeigt. Dieser Entität kann auch verwendet werden, zu einer anderen (modelliert als Dienst principal) Anwendungszugriff auf eine Ressource-Anwendung in einer bestimmten Rolle erteilen. Sie können erstellen, lesen, aktualisieren und Löschen von rollenzuweisungen.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approleassignment"
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
|creationTimestamp|DateTimeOffset|Die Uhrzeit der Erstellung der erteilen. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|id|Guid|Die Rolle-Id, die den Prinzipal zugewiesen wurde.  Diese Rolle muss mit der Ziel-Ressource Anwendung **ResourceId** in seiner **AppRoles** -Eigenschaft deklariert werden. In denen die Ressource keine Berechtigungen nicht deklarieren, muss eine Standard-Id (0 (null) GUID) angegeben werden. Schlüssel. Lässt keine Nullwerte zu. |
|principalDisplayName|String|Der Anzeigename des Prinzipals, die der Zugriff gewährt wurde.|
|principalId|Guid|Der eindeutige Bezeichner (**Id**) für den Prinzipal, den Zugriff gewährt wird. Erforderliche auf erstellen.            |
|principalType|String|Der Typ des Prinzipals.  Dies kann entweder "User", "Group" oder "ServicePrincipal" sein.|
|resourceDisplayName|String|Der Anzeigename der Ressource mit der die Zuordnung hergestellt wurde.|
|resourceId|Guid|Der eindeutige Bezeichner (**Id**) für die Zielressource (Service Principal) für die die Zuordnung erstellt wurde.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von appRoleAssignment](../api/approleassignment-get.md) | [appRoleAssignment](approleassignment.md) |Lesen Sie Eigenschaften und Beziehungen des AppRoleAssignment-Objekts.|
|[Update](../api/approleassignment-update.md) | [appRoleAssignment](approleassignment.md)   |AppRoleAssignment-Objekt zu aktualisieren. |
|[Delete](../api/approleassignment-delete.md) | Keine |AppRoleAssignment-Objekt zu löschen. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->