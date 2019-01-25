---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: publicationFacet
localization_priority: Normal
ms.openlocfilehash: f0887e7ce17a357961c0ee2b19d86388425e82b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513858"
---
# <a name="publicationfacet-resource-type"></a>PublicationFacet-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": [
    "Error: /api-reference/beta/resources/publicationfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
