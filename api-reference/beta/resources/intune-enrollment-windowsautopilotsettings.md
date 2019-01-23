---
title: Ressourcentyp windowsAutopilotSettings
description: Die Ressource WindowsAutopilotSettings stellt ein Windows-Konto Autopilot Synchronisationsdaten mit Windows-Gerät synchronisieren Datendienst dar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cd4641258dbc02829d4b06817467a652de2cb583
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393739"
---
# <a name="windowsautopilotsettings-resource-type"></a>Ressourcentyp windowsAutopilotSettings

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




