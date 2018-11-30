---
title: Ressourcentyp windowsAutopilotSettings
description: Die Ressource WindowsAutopilotSettings stellt ein Windows-Konto Autopilot Synchronisationsdaten mit Windows-Gerät synchronisieren Datendienst dar.
ms.openlocfilehash: 41caab7578be08a56ecad94bbae11c43945037c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062183"
---
# <a name="windowsautopilotsettings-resource-type"></a>Ressourcentyp windowsAutopilotSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource WindowsAutopilotSettings stellt ein Windows-Konto Autopilot Synchronisationsdaten mit Windows-Gerät synchronisieren Datendienst dar.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts.|
|[WindowsAutopilotSettings aktualisieren](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Aktualisieren Sie die Eigenschaften eines [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts.|
|[sync-Aktion](../api/intune-enrollment-windowsautopilotsettings-sync.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|GUID des Objekts|
|lastSyncDateTime|DateTimeOffset|Zuletzt Daten synchronisieren Datum-Uhrzeit mit DDS-Dienst.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Zuletzt Daten synchronisieren Datum-Uhrzeit mit DDS-Dienst.|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Gibt den Status der Synchronisierung mit Gerät Daten Synchronisierungsdiensts (DDS). Mögliche Werte: `unknown`, `inProgress`, `completed`, `failed`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```





