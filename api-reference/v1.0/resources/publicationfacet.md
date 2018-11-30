---
title: PublicationFacet-Ressourcentyp
description: Die **PublicationFacet**-Ressource enthält Details zum veröffentlichten Status einer DriveItemVersion- oder DriveItem-Ressource.
ms.openlocfilehash: 429ec649dc9f511a4012e6790842fdd774bead8b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016581"
---
# <a name="publicationfacet-resource-type"></a>PublicationFacet-Ressourcentyp

Die **PublicationFacet**-Ressource enthält Details zum veröffentlichten Status einer [DriveItemVersion](driveitemversion.md)- oder [DriveItem](driveitem.md)-Ressource.

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a>Eigenschaften

|   Eigenschaft    |  Typ  | Beschreibung |
| :------------ | :----- | :---------- |
| **level**     | string | Der Status der Veröffentlichung für dieses Dokument. Möglich ist `published` oder `checkout`. Schreibgeschützt.  |
| **versionId** | string | Der eindeutige Bezeichner für die Version, die für den aktuellen Anrufer sichtbar ist. Schreibgeschützt.  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
