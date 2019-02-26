---
title: deviceInstallState-Ressourcentyp
description: Enthält Eigenschaften für den Installationsstatus für ein Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c25c9b81be783734f54f4e2edc21f27b070e2ed
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166248"
---
# <a name="deviceinstallstate-resource-type"></a>deviceInstallState-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|deviceName|Zeichenfolge|Name des Geräts|
|deviceId|Zeichenfolge|ID des Geräts|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Synchronisierung|
|installState|[installState](../resources/intune-books-installstate.md)|Installationsstatus des E-Books. Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.|
|errorCode|Zeichenfolge|Fehlercode von Installationsfehlern|
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




