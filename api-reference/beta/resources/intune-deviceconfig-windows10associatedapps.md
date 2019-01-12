---
title: Ressourcentyp windows10AssociatedApps
description: Definition der Windows-10-Anwendung verknüpft ist.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d1f6363027ae46263146efdbf3f5ac5254afcd93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911910"
---
# <a name="windows10associatedapps-resource-type"></a>Ressourcentyp windows10AssociatedApps

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Definition der Windows-10-Anwendung verknüpft ist.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|der appType|[windows10AppType](../resources/intune-deviceconfig-windows10apptype.md)|Anwendungstyp. Mögliche Werte sind: `desktop` und `universal`.|
|Bezeichner|Zeichenfolge|Bezeichner.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```





