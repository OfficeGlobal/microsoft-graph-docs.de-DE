---
title: Connector-Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: eed936c808e920f35a741a836a1fab64b2754bf8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525731"
---
# <a name="connector-resource-type"></a>Connector-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Get-connector](../api/connector-get.md) | Connector |Lesen Sie Eigenschaften und Beziehungen des Connector-Objekts.|
|[memberOf auflisten](../api/connector-list-memberof.md) |[ConnectorGroup](connectorgroup.md) -Auflistung| Ruft das ConnectorGroup-Objekt, das den Connector zugeordnet.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|externalIp|String|Externe IP-Adresse als ermittelte vom Dienst für den Connectorcomputer. Schreibgeschützt|
|id|String| Die Objekt-Id der Verbindung. <BR>Schreibgeschützt.|
|Computername|String| Der Name des Computers, der der Connector ausgeführt wird. <BR>Schreibgeschützt|
|status|string| Gibt den Status der Verbindung. Mögliche Werte sind: `active` und `inactive`. Schreibgeschützt |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|memberOf|[ConnectorGroup](connectorgroup.md) -Auflistung| Die ConnectorGroup, die Verbindung herstellen, ein Mitglied ist.<br>Schreibgeschützt. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connector"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connector.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
