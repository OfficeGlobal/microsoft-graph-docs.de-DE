---
title: Ressourcentyp certificateConnectorSetting
description: Connector-Einstellungen für Zertifikate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 74a63d308d53d09b71b19b2ff10a9d94c3fa818d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980993"
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
|enrollmentError|Zeichenfolge|Zertifikatfehler Connector-Registrierung|
|lastConnectorConnectionTime|DateTimeOffset|Zuletzt Zertifikat Connector verbunden|
|connectorVersion|Zeichenfolge|Version des Zertifikat-Connectors|
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





