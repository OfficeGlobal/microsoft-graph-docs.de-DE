---
title: importedAppleDeviceIdentityResult-Ressourcentyp
description: Die importedAppleDeviceIdentityResult-Ressource stellt das Ergebnis des Versuchs zum Importieren von Apple-Geräte Identitäten dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8a99ffec24825355845f167676eef49205299cf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149462"
---
# <a name="importedappledeviceidentityresult-resource-type"></a>importedAppleDeviceIdentityResult-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die importedAppleDeviceIdentityResult-Ressource stellt das Ergebnis des Versuchs zum Importieren von Apple-Geräte Identitäten dar.


Erbt von [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[ImportedAppleDeviceIdentityResults aufListen](../api/intune-enrollment-importedappledeviceidentityresult-list.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekte.|
|[ImportedAppleDeviceIdentityResult abrufen](../api/intune-enrollment-importedappledeviceidentityresult-get.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Lesen von Eigenschaften und Beziehungen des [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts.|
|[ImportedAppleDeviceIdentityResult erstellen](../api/intune-enrollment-importedappledeviceidentityresult-create.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Erstellen eines neuen [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts.|
|[ImportedAppleDeviceIdentityResult löschen](../api/intune-enrollment-importedappledeviceidentityresult-delete.md)|Keine|Löscht eine [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).|
|[ImportedAppleDeviceIdentityResult aktualisieren](../api/intune-enrollment-importedappledeviceidentityresult-update.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Aktualisieren der Eigenschaften eines [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|Zeichenfolge|Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbte Geräteseriennummer|
|requestedEnrollmentProfileId|Zeichenfolge|Registrierungsprofil-ID, die vom Administrator für das Gerät während der nächsten von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Registrierung angewendet werden soll|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|Das Zeit Registrierungsprofil wurde dem Gerät zugewiesen, das von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbt wurde.|
|isSupervised|Boolescher Wert|Gibt an, ob das Apple-Gerät überwacht wird. Weitere Informationen finden Sie unter https://support.apple.com/en-us/HT202837 : Inherited from [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple-Geräte Ermittlungs Quelle. Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt. Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.|
|createdDateTime|DateTimeOffset|ErstellungsDatum des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts|
|lastContactedDateTime|DateTimeOffset|Datum der letzten Kontaktaufnahme des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts|
|description|Zeichenfolge|Die Beschreibung des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Der Status des Geräts in InTune, das von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt wurde. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|Plattform|[Plattform](../resources/intune-enrollment-platform.md)|Die Plattform des Geräts. Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt. Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.|
|status|Boolescher Wert|Status der importierten Geräte Identität|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
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
  "platform": "String",
  "status": true
}
```




