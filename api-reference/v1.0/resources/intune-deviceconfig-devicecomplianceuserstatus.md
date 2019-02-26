---
title: deviceComplianceUserStatus-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23b72beb38fffbe84dd59f20b93d21bb26897b7c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263308"
---
# <a name="devicecomplianceuserstatus-resource-type"></a>deviceComplianceUserStatus-Ressourcentyp

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



