---
title: Importappledeviceidentitylist-Ressourcentyp
description: Die Importappledeviceidentitylist-Ressource stellt die importierte Geräte Identität eines Apple-Geräts dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5db17bc6a87ab74102126cab3061da5ffbab6fe5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151149"
---
# <a name="importedappledeviceidentity-resource-type"></a>Importappledeviceidentitylist-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Importappledeviceidentitylist-Ressource stellt die importierte Geräte Identität eines Apple-Geräts dar.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[ImportedAppleDeviceIdentities aufListen](../api/intune-enrollment-importedappledeviceidentity-list.md)|[importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekte.|
|[Importappledeviceidentitylist abrufen](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Lesen von Eigenschaften und Beziehungen des [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.|
|[Importappledeviceidentitylist erstellen](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Erstellen eines neuen [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.|
|[Importappledeviceidentitylist löschen](../api/intune-enrollment-importedappledeviceidentity-delete.md)|Keine|Löscht eine [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md).|
|[Importappledeviceidentitylist aktualisieren](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Aktualisieren der Eigenschaften eines [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.|
|[importAppleDeviceIdentityList-Aktion](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|serialNumber|Zeichenfolge|Seriennummer des Geräts|
|requestedEnrollmentProfileId|Zeichenfolge|Registrierungsprofil-ID, die der Administrator während der nächsten Registrierung auf das Gerät anwenden soll|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|Das Zeit Registrierungsprofil wurde dem Gerät zugewiesen|
|isSupervised|Boolean|Gibt an, ob das Apple-Gerät überwacht wird. Weitere Informationen finden Sie unter:https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple-Geräte Ermittlungs Quelle. Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.|
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




