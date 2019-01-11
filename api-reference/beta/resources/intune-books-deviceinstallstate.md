---
title: deviceInstallState-Ressourcentyp
description: Enthält Eigenschaften für den Installationsstatus für ein Gerät.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a407d35189d1b61e870fbdff282a429be165c0c3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819677"
---
# <a name="deviceinstallstate-resource-type"></a>deviceInstallState-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
|id|Zeichenfolge|Schlüssel der Entität|
|deviceName|String|Name des Geräts|
|deviceId|String|ID des Geräts|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Synchronisierung|
|installState|[installState](../resources/intune-books-installstate.md)|Installationsstatus des E-Books. Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.|
|errorCode|String|Fehlercode von Installationsfehlern|
|osVersion|Zeichenfolge|Betriebssystemversion|
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





