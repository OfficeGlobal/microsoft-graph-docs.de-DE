---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: PublicationFacet
ms.openlocfilehash: 60dff1e0dd97073ccb7eccd7be0f51b6b77fc273
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062237"
---
# <a name="publicationfacet-resource-type"></a>PublicationFacet-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
  "tocPath": "Facets/Photo"
} -->
