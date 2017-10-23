---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Foto
ms.openlocfilehash: a4284caa7c20e266d87e22e9b3d729e17bc88abf
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="photo-resource-type"></a>Photo-Ressourcentyp

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
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
