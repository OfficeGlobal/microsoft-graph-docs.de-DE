---
title: Ressourcentyp windowsAppXAppAssignmentSettings
description: Enthält Eigenschaften verwendet, wenn eine AppX Windows mobile app zu einer Gruppe zuweisen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 011bef0bc4ce19028329aff7a4406aea8f918658
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975628"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a>Ressourcentyp windowsAppXAppAssignmentSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften verwendet, wenn eine AppX Windows mobile app zu einer Gruppe zuweisen.

Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|useDeviceContext|Boolescher Wert|Ob Ausführungskontexts Gerät für AppX Windows mobile app verwenden.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





