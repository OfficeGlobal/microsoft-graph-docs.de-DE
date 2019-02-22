---
title: certificateConnectorSetting-Ressourcentyp
description: Zertifikat-konnektoreinstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09f4baf9ddd8be630c432fcec5d7df71c442bbe2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168306"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Zertifikat-konnektoreinstellungen.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|status|Int32|Zertifikat-Connectorstatus|
|certExpiryTime|DateTimeOffset|Dauer des Zertifikats Ablaufs|
|enrollmentError|Zeichenfolge|Zertifikat-Connector-Registrierungsfehler|
|lastConnectorConnectionTime|DateTimeOffset|Letzter Zeitpunkt der Verbindung mit dem Zertifikat-Konnektor|
|connectorVersion|Zeichenfolge|Version von Certificate Connector|
|lastUploadVersion|Int64|Version des zuletzt hochgeladenen Zertifikats-Konnektors|

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




