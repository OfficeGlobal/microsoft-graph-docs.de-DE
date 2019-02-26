---
title: importedDeviceIdentity-Ressourcentyp
description: Die importedDeviceIdentity-Ressource stellt eine eindeutige Hardware Identität eines Geräts dar, das für die Konfiguration vor der Registrierung vorab bereitgestellt wurde.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7ef77b550060d5544a6ee0eda4e6b11923d3571
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151226"
---
# <a name="importeddeviceidentity-resource-type"></a>importedDeviceIdentity-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die importedDeviceIdentity-Ressource stellt eine eindeutige Hardware Identität eines Geräts dar, das für die Konfiguration vor der Registrierung vorab bereitgestellt wurde.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[ImportedDeviceIdentities aufListen](../api/intune-enrollment-importeddeviceidentity-list.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekte.|
|[ImportedDeviceIdentity abrufen](../api/intune-enrollment-importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Lesen von Eigenschaften und Beziehungen des [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.|
|[ImportedDeviceIdentity erstellen](../api/intune-enrollment-importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Erstellen eines neuen [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.|
|[ImportedDeviceIdentity löschen](../api/intune-enrollment-importeddeviceidentity-delete.md)|Keine|Löscht eine [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).|
|[ImportedDeviceIdentity aktualisieren](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Aktualisieren der Eigenschaften eines [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.|
|[importDeviceIdentityList-Aktion](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|ID der importierten Geräte Identität|
|importedDeviceIdentifier|Zeichenfolge|Importierter Gerätebezeichner|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Typ der importierten Geräte Identität. Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Datum der letzten Änderung der Beschreibung|
|createdDateTime|DateTimeOffset|ErstellungsDatum des Geräts|
|lastContactedDateTime|DateTimeOffset|Datum der letzten Kontaktaufnahme des Geräts|
|description|Zeichenfolge|Die Beschreibung des Geräts|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Der Status des Geräts in InTune. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|Plattform|[Plattform](../resources/intune-enrollment-platform.md)|Die Plattform des Geräts. Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




