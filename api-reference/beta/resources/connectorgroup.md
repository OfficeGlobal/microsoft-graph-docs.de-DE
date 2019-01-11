---
title: Ressourcentyp connectorGroup
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 211efe5d8caae57457a6a5cc4fa95d145cd176f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823191"
---
# <a name="connectorgroup-resource-type"></a>Ressourcentyp connectorGroup

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |Lesen Sie Eigenschaften und Beziehungen des ConnectorGroup-Objekts.|
|[Erstellen der Anwendung](../api/connectorgroup-post-applications.md) |[application](application.md)| Ordnen Sie eine Anwendung mit der Connector-Gruppe durch das Veröffentlichen in der Auflistung Applications.|
|[Liste applications](../api/connectorgroup-list-applications.md) |[Application](application.md) -Auflistung| Ruft die Auflistung der verbundenen Anwendung-Objekt.|
|[Erstellen Sie connector](../api/connectorgroup-post-members.md) |[Connector](connector.md)| Hinzufügen einer Verbindung an den Konnektor Gruppe durch die Veröffentlichung auf die Members-Auflistung.|
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
|Elemente|[Connector](connector.md) -Auflistung| Schreibgeschützt. Lässt Nullwerte zu.|

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
<!-- {
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
