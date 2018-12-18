---
title: Ressourcentyp embeddedSIMDeviceState
description: Beschreibt den eingebetteten SIM Code Bereitstellung Aktivierungsstatus in Bezug auf einem Gerät.
author: tfitzmac
ms.openlocfilehash: ef7611e96b1b6f3bba0a3c59dead85ede41b2eda
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308456"
---
# <a name="embeddedsimdevicestate-resource-type"></a>Ressourcentyp embeddedSIMDeviceState

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Beschreibt den eingebetteten SIM Code Bereitstellung Aktivierungsstatus in Bezug auf einem Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste embeddedSIMDeviceStates](../api/intune-esim-embeddedsimdevicestate-list.md)|[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Auflistung|Listeneigenschaften und Beziehungen der [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekte.|
|[Abrufen von embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Lesen Sie Eigenschaften und Beziehungen des [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.|
|[Erstellen von embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Erstellen eines neuen [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.|
|[EmbeddedSIMDeviceState löschen](../api/intune-esim-embeddedsimdevicestate-delete.md)|Keines|Löscht eine [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).|
|[EmbeddedSIMDeviceState aktualisieren](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Aktualisieren Sie die Eigenschaften eines [EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die eingebettete SIM Gerätestatus. System generierten Wert, die beim Erstellen zugewiesen.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt der eingebetteten SIM Gerätestatus erstellt wurde. Generierte Service-Seite.|
|modifiedDateTime|DateTimeOffset|Der Zeitpunkt der letzten Änderung der eingebetteten SIM Gerätestatus. Aktualisierte Service-Seite.|
|lastSyncDateTime|DateTimeOffset|Zeitpunkt, zu das eingebettete SIM Gerät zuletzt eingecheckt. Aktualisierte Service-Seite.|
|universalIntegratedCircuitCardIdentifier|String|Der universelle Chip Karte Bezeichner (UICCID), identifiziert der Hardware, auf der ein Profil ist bereitgestellt werden.|
|deviceName|String|Name des Aufnahmegeräts, dem das Abonnement wurde, bereitgestellt, z. B. DESKTOP JOE|
|userName|String|Benutzernamen, der das Abonnement, z. B. joe@contoso.com bereitgestellt wurde|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|Der Status des Vorgangs Profil angewendet auf das Gerät. Mögliche Werte sind: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted` und `removedByUser`.|
|stateDetails|String|Beschreibung des provisioning Status eine Zeichenfolge.|

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





