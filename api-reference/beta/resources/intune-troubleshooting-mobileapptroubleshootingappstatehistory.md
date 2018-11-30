---
title: Ressourcentyp mobileAppTroubleshootingAppStateHistory
description: Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.
ms.openlocfilehash: 415d018d3650819bce8defe651af8df77e3c6032
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060512"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a>Ressourcentyp mobileAppTroubleshootingAppStateHistory

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Historienelement im Mobile App Problembehandlung Ereignis enthaltenen.

Erbt vom [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|Zeitpunkt, wenn das Historienelement aufgetreten. Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|
|actionType|[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)|AAD Sicherheit Gruppen-Id, der als Ziel angegeben wurde. Mögliche Werte sind: `unknown`, `installCommandSent`, `installed`, `uninstalled` und `userRequestedInstall`.|
|runState|[runState](../resources/intune-shared-runstate.md)|Status des Elements. Mögliche Werte sind: `unknown`, `success` und `fail`.|
|errorCode|String|Der Fehlercode des Fehlers, leer, wenn kein Fehler.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```





