---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Paket
localization_priority: Normal
ms.openlocfilehash: bcfc1a1e754286566c8b24b9b00c7f2eb0721316
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482385"
---
# <a name="package-resource-type"></a>Package-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **Package**-Ressource gibt an, dass ein DriveItem das Element der obersten Ebene in einem „Paket“ oder einer Sammlung von Elementen ist, die als eine Sammlung und nicht als einzelne Elemente behandelt werden müssen.

Ein Beispiel für ein Paket ist ein OneNote-Notizbuch. Während das Notizbuch aus Dateien und Ordnern besteht, die die Inhalte des Notizbuchs darstellen, weist das Element der obersten Ebene, das das Notizbuch darstellt, ein **package**-Facet auf, um für Clients anzugeben, dass es sich dabei um eine Sammlung von Daten handelt, die auf besondere Weise behandelt werden müssen.

DriveItems mit dem **package**-Facet enthalten keine **folder**- oder **file**-Facets, sie ähneln jedoch Elementen mit einem **folder**-Facet.

## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| Eigenschaftenname | Typ   | Beschreibung                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **type**      | string | Eine Zeichenfolge, die den Typ des Pakets angibt. Obwohl `oneNote` der einzige derzeit definierte Wert ist, sollten Sie davon ausgehen, dass andere Paketarten zurückgegeben werden, die entsprechend behandelt werden müssen. |

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).


<!--
{
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/package.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
