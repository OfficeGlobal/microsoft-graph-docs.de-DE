---
title: Ressourcentyp resourceAccess
description: Gibt ein Berechtigungsbereich OAuth 2.0 oder eine app-Rolle, die eine Anwendung funktioniert. Die **ResourceAccess** -Eigenschaft vom Typ RequiredResourceAccess ist eine Auflistung von **ResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: 1e741aa49e56b304c265a5fd701fdac37feb29dd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519024"
---
# <a name="resourceaccess-resource-type"></a>Ressourcentyp resourceAccess

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gibt ein Berechtigungsbereich OAuth 2.0 oder eine app-Rolle, die eine Anwendung funktioniert. Die **ResourceAccess** -Eigenschaft vom Typ [RequiredResourceAccess](requiredresourceaccess.md) ist eine Auflistung von **ResourceAccess**.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|Guid|Der eindeutige Bezeichner für eine der [oAuth2Permission](oauth2permission.md) oder [AppRole](approle.md) -Instanzen, die die Anwendung für die Ressource verfügbar macht.|
|type|String|Gibt an, ob die **Id** -Eigenschaft ein [oAuth2Permission](oauth2permission.md) oder ein [AppRole](approle.md)verweist. Mögliche Werte sind "Bereich" oder "Rolle".|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
