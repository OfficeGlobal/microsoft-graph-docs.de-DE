---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Foto
localization_priority: Normal
ms.openlocfilehash: 91b893fe3d6c78e3c3e16cbc41c7d7543b08f8d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527626"
---
# <a name="photo-resource-type"></a>Photo-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **photo**-Ressource stellt Foto- und Kameraeigenschaften auf einem [DriveItem](driveitem.md) bereit, z. B. EXIF-Metadaten.

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft                | Typ           | Beschreibung
|:------------------------|:---------------|:----------------------------------
| **takenDateTime**       | DateTimeOffset | Stellt das Datum und die Uhrzeit für die Aufnahme des Fotos dar. Schreibgeschützt.
| **cameraMake**          | String         | Kamerahersteller Schreibgeschützt.
| **cameraModel**         | String         | Kameramodell. Schreibgeschützt.
| **fNumber**             | Gleitkommawert mit doppelter Genauigkeit         | Die Blendenzahl der Kamera. Schreibgeschützt.
| **exposureDenominator** | Gleitkommawert mit doppelter Genauigkeit         | Der Nenner der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt.
| **exposureNumerator**   | Gleitkommawert mit doppelter Genauigkeit         | Der Zähler der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt.
| **focalLength**         | Gleitkommawert mit doppelter Genauigkeit         | Die Brennweite der Kamera. Schreibgeschützt.
| **iso**                 | Int64          | Der ISO-Wert der Kamera. Schreibgeschützt.

## <a name="remarks"></a>Bemerkungen
Von OneDrive for Business und SharePoint wird nur die **TakenDateTime**-Eigenschaft zurückgegeben.

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).
<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": [
    "Error: /api-reference/beta/resources/photo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
