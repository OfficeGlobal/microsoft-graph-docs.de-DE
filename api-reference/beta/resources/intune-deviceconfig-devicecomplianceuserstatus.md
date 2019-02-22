---
title: deviceComplianceUserStatus-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 55fb7695c24a22c5fcec96afd67c483b42ce905e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175269"
---
# <a name="devicecomplianceuserstatus-resource-type"></a>deviceComplianceUserStatus-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Noch nicht dokumentiert.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceComplianceUserStatuses auflisten](../api/intune-deviceconfig-devicecomplianceuserstatus-list.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)-Objekte.|
|[deviceComplianceUserStatus abrufen](../api/intune-deviceconfig-devicecomplianceuserstatus-get.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Lesen von Eigenschaften und Beziehungen des [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)-Objekts.|
|[DeviceComplianceUserStatus erstellen](../api/intune-deviceconfig-devicecomplianceuserstatus-create.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Erstellen eines neuen [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)-Objekts.|
|[DeviceComplianceUserStatus löschen](../api/intune-deviceconfig-devicecomplianceuserstatus-delete.md)|Keine|Löscht ein [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)-Objekt.|
|[DeviceComplianceUserStatus aktualisieren](../api/intune-deviceconfig-devicecomplianceuserstatus-update.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Aktualisieren der Eigenschaften eines [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|userDisplayName|String|Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört|
|devicesCount|Int32|Geräteanzahl für den Benutzer|
|status|[Wurde](../resources/intune-shared-compliancestatus.md)|Konformitätsstatus des Richtlinienberichts. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Richtlinienberichts|
|userPrincipalName|Zeichenfolge|Benutzer-Prinzipalname|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```




