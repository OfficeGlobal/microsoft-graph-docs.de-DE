---
title: Ressourcentyp deviceManagementScriptRunSummary
description: Enthält Eigenschaften für die Laufzeit Zusammenfassung für ein Gerät Management-Skript.
ms.openlocfilehash: 9269ae5f3f6fc889cb02ad90e2897c9a3e979241
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063945"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a>Ressourcentyp deviceManagementScriptRunSummary

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für die Laufzeit Zusammenfassung für ein Gerät Management-Skript.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von deviceManagementScriptRunSummary](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.|
|[DeviceManagementScriptRunSummary aktualisieren](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Das Gerät Management-Skript ausführen Zusammenfassung Entität-Taste.|
|successDeviceCount|Int32|Anzahl der Geräte Erfolg.|
|errorDeviceCount|Int32|Anzahl der Fehler Geräte.|
|successUserCount|Int32|Benutzeranzahl Erfolg.|
|errorUserCount|Int32|Anzahl der Fehler Benutzer.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```




