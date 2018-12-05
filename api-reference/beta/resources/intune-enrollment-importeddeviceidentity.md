---
title: Ressourcentyp importedDeviceIdentity
description: Die Ressource ImportedDeviceIdentity stellt eine eindeutige Hardware Identität eines Geräts für die Konfiguration der Registrierung vor dem bereits bereitgestellt wurde.
ms.openlocfilehash: a327840ce38dfd0d075ef37c7e92ef0e83b2054c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065621"
---
# <a name="importeddeviceidentity-resource-type"></a>Ressourcentyp importedDeviceIdentity

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource ImportedDeviceIdentity stellt eine eindeutige Hardware Identität eines Geräts für die Konfiguration der Registrierung vor dem bereits bereitgestellt wurde.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste importedDeviceIdentities](../api/intune-enrollment-importeddeviceidentity-list.md)|[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Auflistung|Listeneigenschaften und Beziehungen der [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekte.|
|[Abrufen von importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Lesen Sie Eigenschaften und Beziehungen des [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.|
|[Erstellen von importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Erstellen eines neuen [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.|
|[ImportedDeviceIdentity löschen](../api/intune-enrollment-importeddeviceidentity-delete.md)|Keines|Löscht eine [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).|
|[ImportedDeviceIdentity aktualisieren](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Aktualisieren Sie die Eigenschaften eines [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.|
|[ImportDeviceIdentityList Aktion](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Auflistung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|ID der Identität des importierten Geräts|
|importedDeviceIdentifier|String|Importierte Geräte-ID|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Art der importierten Gerät Identität. Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Letzte Änderung DateTime der Beschreibung|
|createdDateTime|DateTimeOffset|Erstellte Datum-Uhrzeit des Geräts|
|lastContactedDateTime|DateTimeOffset|Letzte kontaktiert Datum-Uhrzeit des Geräts|
|description|String|Die Beschreibung des Geräts|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Der Zustand des Geräts in Intune. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
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




