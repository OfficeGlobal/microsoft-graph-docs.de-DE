---
title: embeddedSIMDeviceState-Ressourcentyp
description: Beschreibt den bereit stellungs Status der eingebetteten SIM-Aktivierungscode in Bezug auf ein Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c358fb343282bdb30b43226a02fe127c73613dcc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151058"
---
# <a name="embeddedsimdevicestate-resource-type"></a>embeddedSIMDeviceState-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Beschreibt den bereit stellungs Status der eingebetteten SIM-Aktivierungscode in Bezug auf ein Gerät.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[EmbeddedSIMDeviceStates aufListen](../api/intune-esim-embeddedsimdevicestate-list.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekte.|
|[EmbeddedSIMDeviceState abrufen](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Lesen von Eigenschaften und Beziehungen des [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.|
|[EmbeddedSIMDeviceState erstellen](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Erstellen eines neuen [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.|
|[EmbeddedSIMDeviceState löschen](../api/intune-esim-embeddedsimdevicestate-delete.md)|Keine|Löscht eine [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).|
|[EmbeddedSIMDeviceState aktualisieren](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Aktualisieren der Eigenschaften eines [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für den Status des eingebetteten SIM-Geräts. Vom System generierter Wert, der bei der Erstellung zugewiesen wird.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu dem der Status des eingebetteten SIM-Geräts erstellt wurde. Generierte Dienstseite.|
|modifiedDateTime|DateTimeOffset|Zeitpunkt, zu dem der Status des eingebetteten SIM-Geräts zuletzt geändert wurde. Aktualisierte Dienstseite.|
|lastSyncDateTime|DateTimeOffset|Zeitpunkt, zu dem das eingebettete SIM-Gerät zuletzt eingecheckt hat. Aktualisierte Dienstseite.|
|universalIntegratedCircuitCardIdentifier|Zeichenfolge|Der universelle integrierte Leiterkarten Bezeichner (UICCID), der die Hardware identifiziert, auf der ein Profil bereitgestellt werden soll.|
|deviceName|Zeichenfolge|Gerätename, für den das Abonnement vorgesehen wurde (z. b. DESKTOP-JOE)|
|userName|Zeichenfolge|Benutzername, für den das Abonnement z. b. joe@contoso.com wurde|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|Der Status des auf das Gerät angewendeten Profil Vorgangs. Mögliche Werte sind: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted` und `removedByUser`.|
|stateDetails|Zeichenfolge|Beschreibung des Zustands der Einrichtung.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "universalIntegratedCircuitCardIdentifier": "String",
  "deviceName": "String",
  "userName": "String",
  "state": "String",
  "stateDetails": "String"
}
```




