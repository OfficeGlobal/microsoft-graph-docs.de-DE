---
title: Ressourcentyp embeddedSIMDeviceState
description: Beschreibt den eingebetteten SIM Code Bereitstellung Aktivierungsstatus in Bezug auf einem Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ce96250b8c64fc97171ee7721ca44b4cd4579072
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912624"
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





