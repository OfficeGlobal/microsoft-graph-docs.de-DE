---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: d49142ed414ad82ec149792e11e5a8c42d9837dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852640"
---
# <a name="geocoordinates-resource-type"></a>GeoCoordinates-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **GeoCoordinates**-Ressource liefert geografische Koordinaten und die Erhebung eines Orts basierend auf Metadaten, die in der Datei enthalten sind. Wenn ein [**DriveItem**](driveitem.md) ein **location**-Facet ungleich Null aufweist, stellt das Element eine Datei dar, die mit einem bekannten Ort verknüpft ist.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft  | Typ   | Beschreibung
|:----------|:-------|:--------------------------------------------------------
| altitude  | Gleitkommawert mit doppelter Genauigkeit | Optional. Die Höhe oberhalb des Meeresspiegels in Fuß. Schreibgeschützt.
| latitude  | Gleitkommawert mit doppelter Genauigkeit | Optional. Der Breitengrad für das Element als Kommazahl. Schreibgeschützt.
| longitude | Gleitkommawert mit doppelter Genauigkeit | Optional. Der Längengrad für das Element als Kommazahl. Schreibgeschützt.

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
