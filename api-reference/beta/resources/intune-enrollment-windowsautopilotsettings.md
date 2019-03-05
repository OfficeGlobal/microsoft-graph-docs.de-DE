---
title: windowsAutopilotSettings-Ressourcentyp
description: Die windowsAutopilotSettings-Ressource stellt ein Windows Autopilot-Konto zum Synchronisieren von Daten mit dem Windows-Gerätedaten-Synchronisierungsdienst dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b34d6edbed5bc98989ea70186b081d5c88a1c1b6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140516"
---
# <a name="windowsautopilotsettings-resource-type"></a>windowsAutopilotSettings-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die windowsAutopilotSettings-Ressource stellt ein Windows Autopilot-Konto zum Synchronisieren von Daten mit dem Windows-Gerätedaten-Synchronisierungsdienst dar.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsAutopilotSettings abrufen](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Lesen von Eigenschaften und Beziehungen des [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts.|
|[WindowsAutopilotSettings aktualisieren](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Aktualisieren der Eigenschaften eines [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts.|
|[sync-Aktion](../api/intune-enrollment-windowsautopilotsettings-sync.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|GUID des Objekts|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Datensynchronisierung mit dem DDS-Dienst.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Datensynchronisierung mit dem DDS-Dienst.|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Gibt den Status der Synchronisierung mit Device Data Sync (DDS)-Dienst an. Mögliche Werte: `unknown`, `inProgress`, `completed`, `failed`.|

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




