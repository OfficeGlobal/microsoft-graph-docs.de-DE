---
title: deviceInstallState-Ressourcentyp
description: Enthält Eigenschaften für den Installationsstatus für ein Gerät.
author: tfitzmac
ms.openlocfilehash: 660ecb3dfae66e2f442027f61b82da69c2cee286
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354593"
---
# <a name="deviceinstallstate-resource-type"></a>deviceInstallState-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für den Installationsstatus für ein Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceInstallStates auflisten](../api/intune-books-deviceinstallstate-list.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekte.|
|[deviceInstallState abrufen](../api/intune-books-deviceinstallstate-get.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Lesen von Eigenschaften und Beziehungen des [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekts.|
|[deviceInstallState erstellen](../api/intune-books-deviceinstallstate-create.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Erstellen eines neuen [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekts.|
|[deviceInstallState löschen](../api/intune-books-deviceinstallstate-delete.md)|Keine|Löscht ein [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekt.|
|[deviceInstallState aktualisieren](../api/intune-books-deviceinstallstate-update.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Aktualisieren der Eigenschaften eines [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|deviceName|String|Name des Geräts|
|deviceId|String|ID des Geräts|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Synchronisierung|
|installState|[installState](../resources/intune-books-installstate.md)|Installationsstatus des E-Books. Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.|
|errorCode|String|Fehlercode von Installationsfehlern|
|osVersion|String|Betriebssystemversion|
|osDescription|String|Beschreibung des Betriebssystems|
|userName|String|Benutzername des Geräts|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



