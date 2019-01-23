---
title: Ressourcentyp embeddedSIMDeviceState
description: Beschreibt den eingebetteten SIM Code Bereitstellung Aktivierungsstatus in Bezug auf einem Gerät.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a79453c8d8bcb5682da64ce480f1a2f9f210a673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415572"
---
# <a name="embeddedsimdevicestate-resource-type"></a>Ressourcentyp embeddedSIMDeviceState

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Beschreibt den eingebetteten SIM Code Bereitstellung Aktivierungsstatus in Bezug auf einem Gerät.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste embeddedSIMDeviceStates](../api/intune-esim-embeddedsimdevicestate-list.md)|[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Auflistung|Listeneigenschaften und Beziehungen der [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekte.|
|[Abrufen von embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Lesen Sie Eigenschaften und Beziehungen des [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.|
|[Erstellen von embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Erstellen eines neuen [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.|
|[EmbeddedSIMDeviceState löschen](../api/intune-esim-embeddedsimdevicestate-delete.md)|Keine|Löscht eine [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).|
|[EmbeddedSIMDeviceState aktualisieren](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Aktualisieren Sie die Eigenschaften eines [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für die eingebettete SIM Gerätestatus. System generierten Wert, die beim Erstellen zugewiesen.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt der eingebetteten SIM Gerätestatus erstellt wurde. Generierte Service-Seite.|
|modifiedDateTime|DateTimeOffset|Der Zeitpunkt der letzten Änderung der eingebetteten SIM Gerätestatus. Aktualisierte Service-Seite.|
|lastSyncDateTime|DateTimeOffset|Zeitpunkt, zu das eingebettete SIM Gerät zuletzt eingecheckt. Aktualisierte Service-Seite.|
|universalIntegratedCircuitCardIdentifier|Zeichenfolge|Der universelle Chip Karte Bezeichner (UICCID), identifiziert der Hardware, auf der ein Profil ist bereitgestellt werden.|
|deviceName|Zeichenfolge|Name des Aufnahmegeräts, dem das Abonnement wurde, bereitgestellt, z. B. DESKTOP JOE|
|userName|Zeichenfolge|Benutzernamen, der das Abonnement, z. B. joe@contoso.com bereitgestellt wurde|
|Zustand|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|Der Status des Vorgangs Profil angewendet auf das Gerät. Mögliche Werte sind: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted` und `removedByUser`.|
|stateDetails|Zeichenfolge|Beschreibung des provisioning Status eine Zeichenfolge.|

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




