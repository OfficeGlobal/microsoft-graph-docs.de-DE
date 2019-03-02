---
title: dimensionValues-Ressourcentyp
description: Ein Dimensionswert in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: da3935b8e784b05551af123c1832d5dc84a2c81c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365318"
---
# <a name="dimensionvalues-resource-type"></a>dimensionValues-Ressourcentyp
Stellt einen Dimensionswert in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung                   |
|:-------------|:-------------|:-----------------------------|
|[DimensionValues abrufen](../api/dynamics-dimensionvalue-get.md)|dimensionValues|Ruft ein Dimensionswert Objekt ab.|


## <a name="properties"></a>Eigenschaften
| Eigenschaft           | Typ                  |Beschreibung                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|id                  |GUID                   |Die eindeutige ID des Elements.                         |
|code                |Zeichenfolge, maximale Größe 20|Der Dimensionswertcode.                          |
|displayName         |string                 |Gibt den Namen des Dimensionswerts an. Dieser Name wird angezeigt, wenn der Dimensionswert verwendet wird.|
|lastModifiedDateTime|DateTime               |Die letzte DateTime, für die der Dimensionswert geändert wurde.|  


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


