---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Foto
ms.openlocfilehash: f61d37eecccd4bf08a2f8abbf4cda15dee5eb94d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062025"
---
# <a name="photo-resource-type"></a>Photo-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
