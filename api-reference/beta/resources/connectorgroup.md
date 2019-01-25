---
title: Ressourcentyp connectorGroup
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517498"
---
# <a name="connectorgroup-resource-type"></a>Ressourcentyp connectorGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |Lesen Sie Eigenschaften und Beziehungen des ConnectorGroup-Objekts.|
|[Erstellen der Anwendung](../api/connectorgroup-post-applications.md) |[application](application.md)| Ordnen Sie eine Anwendung mit der Connector-Gruppe durch das Veröffentlichen in der Auflistung Applications.|
|[Liste applications](../api/connectorgroup-list-applications.md) |[Application](application.md) -Auflistung| Ruft die Auflistung der verbundenen Anwendung-Objekt.|
|[Erstellen Sie connector](../api/connectorgroup-post-members.md) |Connector| Hinzufügen einer Verbindung an den Konnektor Gruppe durch die Veröffentlichung auf die Members-Auflistung.|
|[Mitglieder auflisten](../api/connectorgroup-list-members.md) |[Connector](connector.md) -Auflistung| Rufen Sie einen Connector-Auflistung-Objekts.|
|[Update](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)    |ConnectorGroup-Objekt zu aktualisieren. |
|[Delete](../api/connectorgroup-delete.md) | Keine |ConnectorGroup-Objekt zu löschen. Sämtliche Verbinder muss entfernen, bevor eine Gruppe Connector gelöscht werden kann. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|connectorGroupType|string| Der Typ des Connectors, die mit der Gruppe verwendet werden. Mögliche Werte sind: `applicationProxy`.|
|id|String| Die Objekt-Id der connectorGroup|
|isDefault|Boolescher Wert| Gibt an, ob die ConnectorGroup der Standardgruppe Connector. Nur ein einzelner Connector Gruppe kann die Standard-ConnectorGroup und wird vom System festgelegt.|
|name|Zeichenfolge| Der Name der ConnectorGroup zugeordnet.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Anwendungen|[Application](application.md) -Auflistung| Schreibgeschützt. Lässt Nullwerte zu.|
|members|[Connector](connector.md) -Auflistung| Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connectorgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
