---
title: Ressourcentyp windows10AppsForceUpdateSchedule
description: Zeitplan für die Aktualisierung von Windows 10 Force für Apps
ms.openlocfilehash: 89bbee05c3a76df6999c0d3d16caa591f903c45a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062050"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a>Ressourcentyp windows10AppsForceUpdateSchedule

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zeitplan für die Aktualisierung von Windows 10 Force für Apps
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|startDateTime|DateTimeOffset|Starten Sie die Startzeit für die Force neu.|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|Serie planen. Mögliche Werte: sind `none`, `daily`, `weekly` und `monthly`.|
|runImmediatelyIfAfterStartDateTime|Boolesch|Bei true wird die Aufgabe sofort ausgeführt, wenn StartDateTime in der Vergangenheit andere Person ist, wird zur nächsten Serie ausgeführt wird.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```





