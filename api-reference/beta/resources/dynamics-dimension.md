---
title: Dimensions-Ressourcentyp
description: Eine Dimension in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 92ba48a7ad55b6a7dff28ccc1547769c149e378b
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365570"
---
# <a name="dimensions-resource-type"></a>Dimensions-Ressourcentyp
Stellt eine Dimension in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden
| Methode       | Rückgabetyp  |Beschreibung|
|:-------------|:-------------|:----------|
|[Dimensionen abrufen](../api/dynamics-dimension-get.md)|dimension|Ruft eine Dimension ab.|


## <a name="properties"></a>Eigenschaften
| Eigenschaft           | Typ                  |Beschreibung               |
|:-------------------|:----------------------|:-------------------------|
|id                  |GUID                   |Die eindeutige ID des Elements.|
|code                |Zeichenfolge, maximale Größe 20|Der Dimensionscode.       |
|displayName         |string                 |Gibt den Namen der Dimension an. Dieser Name wird angezeigt, wo die Dimension verwendet wird.|
|lastModifiedDateTime|DateTime               |Die letzte DateTime, die die Dimension geändert wurde.|  


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

