---
title: Ressourcentyp officeConfigurationGroupAssignmentTarget
description: Office-Client-Konfiguration AAD Zuordnung Ziel gruppieren
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9d59a6adc5478d619187e5414ac92170cbdedd49
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926379"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a>Ressourcentyp officeConfigurationGroupAssignmentTarget

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Office-Client-Konfiguration AAD Zuordnung Ziel gruppieren

Erbt vom [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|groupId|Zeichenfolge|Die Id der Gruppe AAD sind wir Gerätekonfiguration zu adressieren.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



