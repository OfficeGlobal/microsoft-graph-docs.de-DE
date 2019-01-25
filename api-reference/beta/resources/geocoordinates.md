---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: 45df506820ee242b53630c9d44ed390216bae141
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525073"
---
# <a name="geocoordinates-resource-type"></a>GeoCoordinates-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location",
  "suppressions": [
    "Error: /api-reference/beta/resources/geocoordinates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
