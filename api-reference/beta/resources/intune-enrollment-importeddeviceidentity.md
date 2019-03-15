---
title: importedDeviceIdentity-Ressourcentyp
description: Die importedDeviceIdentity-Ressource stellt eine eindeutige Hardware Identität eines Geräts dar, das für die Konfiguration vor der Registrierung vorab bereitgestellt wurde.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f5dcc3d7ef6cb59bffe1d7b8cfda958e76c3e35
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572103"
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
|[ImportedDeviceIdentity löschen](../api/intune-enrollment-importeddeviceidentity-delete.md)|None|Löscht eine [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).|
|[ImportedDeviceIdentity aktualisieren](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Aktualisieren der Eigenschaften eines [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.|
|[importDeviceIdentityList-Aktion](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Sammlung|Noch nicht dokumentiert.|
|[searchExistingIdentities-Aktion](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Sammlung|Noch nicht dokumentiert.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|ID der importierten Geräte Identität|
|importedDeviceIdentifier|String|Importierter Gerätebezeichner|
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




