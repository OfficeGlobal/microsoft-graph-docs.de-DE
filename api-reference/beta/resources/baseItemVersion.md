---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 56a2c230c53c4b5bd50e8c123dd69eedec67a141
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480670"
---
# <a name="baseitemversion-resource-type"></a>BaseItemVersion-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **baseItemVersion**-Ressource stellt eine frühere Version eines Elements oder einer Entität dar.


## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.baseItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>Eigenschaften

|      Eigenschaftenname       |                         Typ                         |                               Beschreibung                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | Die ID der Version. Schreibgeschützt.                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | Die Identität des Benutzers, der die Version zuletzt geändert hat. Schreibgeschützt.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Datum und Uhrzeit der letzten Änderung der Version. Schreibgeschützt.                 |
| **Veröffentlichung**          | [PublicationFacet](../resources/publicationfacet.md) | Zeigt den Veröffentlichungsstatus dieser bestimmten Version an. Schreibgeschützt. |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
