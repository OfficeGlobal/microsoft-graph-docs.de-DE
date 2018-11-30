---
title: Connector-Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 6d4cb7e5ca1a5384dbb6c8be92e7ce4eb107388a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064598"
---
# <a name="connector-resource-type"></a>Connector-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Get-connector](../api/connector-get.md) | [Connector](connector.md) |Lesen Sie Eigenschaften und Beziehungen des Connector-Objekts.|
|[memberOf auflisten](../api/connector-list-memberof.md) |[ConnectorGroup](connectorgroup.md) -Auflistung| Ruft das ConnectorGroup-Objekt, das den Connector zugeordnet.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|externalIp|String|Externe IP-Adresse als ermittelte vom Dienst für den Connectorcomputer. Schreibgeschützt.|
|id|String| Die Objekt-Id der Verbindung. <BR>Schreibgeschützt.|
|Computername|String| Der Name des Computers, der der Connector ausgeführt wird. <BR>Schreibgeschützt.|
|status|string| Gibt den Status der Verbindung. Mögliche Werte sind: `active` und `inactive`. Schreibgeschützt. |

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
<!-- {
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
