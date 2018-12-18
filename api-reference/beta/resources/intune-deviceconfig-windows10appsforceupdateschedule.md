---
title: Ressourcentyp windows10AppsForceUpdateSchedule
description: Zeitplan für die Aktualisierung von Windows 10 Force für Apps
author: tfitzmac
ms.openlocfilehash: 851f22e092f2669dfc44911783df6182cda1dc6d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323702"
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





