---
title: Connector-Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 98fa998a37b01ad64e556b229912932f4d1cfc75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884623"
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
|externalIp|Zeichenfolge|Externe IP-Adresse als ermittelte vom Dienst für den Connectorcomputer. Schreibgeschützt.|
|id|Zeichenfolge| Die Objekt-Id der Verbindung. <BR>Schreibgeschützt.|
|Computername|Zeichenfolge| Der Name des Computers, der der Connector ausgeführt wird. <BR>Schreibgeschützt.|
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
