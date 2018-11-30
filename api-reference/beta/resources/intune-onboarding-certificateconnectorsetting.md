---
title: Ressourcentyp certificateConnectorSetting
description: Connector-Einstellungen für Zertifikate.
ms.openlocfilehash: 65f87002016c4d5bd6b19106ba1aa988ad30d92e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057903"
---
# <a name="certificateconnectorsetting-resource-type"></a>Ressourcentyp certificateConnectorSetting

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Connector-Einstellungen für Zertifikate.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|status|Int32|Zertifikat Connectorstatus|
|certExpiryTime|DateTimeOffset|Zertifikat abläuft Zeit|
|enrollmentError|String|Zertifikatfehler Connector-Registrierung|
|lastConnectorConnectionTime|DateTimeOffset|Zuletzt Zertifikat Connector verbunden|
|connectorVersion|String|Version des Zertifikat-Connectors|
|lastUploadVersion|Int64|Version des letzten hochgeladenen Zertifikat connector|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```





