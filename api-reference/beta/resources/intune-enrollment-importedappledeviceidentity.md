---
title: Ressourcentyp importedAppleDeviceIdentity
description: Die Ressource ImportedAppleDeviceIdentity stellt die Identität des importierten Geräts von einem Apple-Gerät.
author: tfitzmac
ms.openlocfilehash: 966e384b63026def366ba19ea634d635d77d9083
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317591"
---
# <a name="importedappledeviceidentity-resource-type"></a>Ressourcentyp importedAppleDeviceIdentity

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource ImportedAppleDeviceIdentity stellt die Identität des importierten Geräts von einem Apple-Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste importedAppleDeviceIdentities](../api/intune-enrollment-importedappledeviceidentity-list.md)|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Auflistung|Listeneigenschaften und Beziehungen der [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekte.|
|[Abrufen von importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Lesen Sie Eigenschaften und Beziehungen des [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.|
|[Erstellen von importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Erstellen eines neuen [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.|
|[ImportedAppleDeviceIdentity löschen](../api/intune-enrollment-importedappledeviceidentity-delete.md)|Keines|Löscht eine [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).|
|[ImportedAppleDeviceIdentity aktualisieren](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Aktualisieren Sie die Eigenschaften eines [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.|
|[ImportAppleDeviceIdentityList Aktion](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|[ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Auflistung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|serialNumber|String|Seriennummer des Geräts|
|requestedEnrollmentProfileId|String|Registrierung Profil Id Admin beabsichtigt, auf dem Gerät während der nächsten Registrierung anwenden|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|Das Zeit Registrierung Profil zugewiesen wurde das Gerät|
|isSupervised|Boolescher Wert|Gibt an, ob das Gerät Apple überwacht wird. Weitere Informationen finden Sie unter:https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple Gerät Discovery-Quelle. Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.|
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
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "String (identifier)",
  "serialNumber": "String",
  "requestedEnrollmentProfileId": "String",
  "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
  "isSupervised": true,
  "discoverySource": "String",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```





