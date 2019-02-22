---
title: importedDeviceIdentityResult-Ressourcentyp
description: Die importedDeviceIdentityResult-Ressource stellt das Ergebnis der Versuch, eine Geräte Identität zu importieren.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b1a5fbaac297a85595827f23cafd93035188bc4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156280"
---
# <a name="importeddeviceidentityresult-resource-type"></a>importedDeviceIdentityResult-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die importedDeviceIdentityResult-Ressource stellt das Ergebnis der Versuch, eine Geräte Identität zu importieren.


Erbt von [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[ImportedDeviceIdentityResults aufListen](../api/intune-enrollment-importeddeviceidentityresult-list.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekte.|
|[ImportedDeviceIdentityResult abrufen](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Lesen von Eigenschaften und Beziehungen des [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekts.|
|[ImportedDeviceIdentityResult erstellen](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Erstellen eines neuen [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekts.|
|[ImportedDeviceIdentityResult löschen](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|Keine|Löscht eine [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).|
|[ImportedDeviceIdentityResult aktualisieren](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Aktualisieren der Eigenschaften eines [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|ID der von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten importierten Geräte Identität|
|importedDeviceIdentifier|Zeichenfolge|Von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbte importierte Gerätebezeichner|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Typ der importierten Geräte Identität, die von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt wurde. Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Datum der letzten Änderung der von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Beschreibung|
|createdDateTime|DateTimeOffset|ErstellungsDatum des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts|
|lastContactedDateTime|DateTimeOffset|Datum der letzten Kontaktaufnahme des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts|
|description|Zeichenfolge|Die Beschreibung des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Der Status des Geräts in InTune, das von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt wurde. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|Plattform|[Plattform](../resources/intune-enrollment-platform.md)|Die Plattform des Geräts. Von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt. Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.|
|status|Boolescher Wert|Status der importierten Geräte Identität|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```




