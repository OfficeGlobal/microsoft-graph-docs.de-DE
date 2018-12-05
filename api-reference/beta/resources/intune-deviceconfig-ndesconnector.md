---
title: Ressourcentyp ndesConnector
description: Die Entität, die einen OnPrem Ndes Connector darstellt.
ms.openlocfilehash: d8cce2601f0f51703cccabe0690165e67b0af2bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058624"
---
# <a name="ndesconnector-resource-type"></a>Ressourcentyp ndesConnector

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Entität, die einen OnPrem Ndes Connector darstellt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste ndesConnectors](../api/intune-deviceconfig-ndesconnector-list.md)|[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Auflistung|Listeneigenschaften und Beziehungen der [NdesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekte.|
|[Abrufen von ndesConnector](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Lesen Sie Eigenschaften und Beziehungen des [NdesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekts.|
|[Erstellen von ndesConnector](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Erstellen eines neuen [NdesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekts.|
|[NdesConnector löschen](../api/intune-deviceconfig-ndesconnector-delete.md)|Keines|Löscht eine [NdesConnector](../resources/intune-deviceconfig-ndesconnector.md).|
|[NdesConnector aktualisieren](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Aktualisieren Sie die Eigenschaften eines [NdesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Der Schlüssel des NDES Connectors.|
|lastConnectionDateTime|DateTimeOffset|Letzte Verbindungszeit für den Ndes Connector|
|state|[ndesConnectorState](../resources/intune-deviceconfig-ndesconnectorstate.md)|NDES Connector Status. Mögliche Werte sind: `none`, `active` und `inactive`.|
|displayName|String|Der Anzeigename der Verbindung Ndes.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ndesConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "String (identifier)",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "displayName": "String"
}
```




