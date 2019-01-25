---
author: rgregg
ms.author: rgregg
ms.date: 09/14/2017
title: Identität
localization_priority: Normal
ms.openlocfilehash: 1ac2aea59ab0d6b09ae613b72fbfbf924240a4a0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518793"
---
# <a name="identity-resource-type"></a>Identität Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **Identity**-Ressource stellt eine Identität von einem _Akteur_ dar. Ein Akteur kann z. B. ein Benutzer, Gerät oder eine Anwendung sein.

## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ   | Beschreibung                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName         | Zeichenfolge | Der Anzeigenamen der Identität. Beachten Sie, dass dieser möglicherweise nicht immer verfügbar oder auf dem neuesten Stand ist. Wenn sich z. B. der Anzeigename eines Benutzers ändert, zeigt die API möglicherweise den neuen Wert in einer zukünftigen Antwort an, aber für die dem Benutzer zugeordneten Elemente wird mit [delta](../api/driveitem-delta.md) nicht angezeigt, dass sie sich geändert haben.  |
| id                  | String | Eindeutiger Bezeichner für die Identität.                                                                                                                                                                                                                                                                                   |
| tenantId            | String | Eindeutige Identität des Mandanten (optional).                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a>Bemerkungen

Unter gewissen Umständen steht der eindeutige Bezeichner für den Akteur möglicherweise nicht zur Verfügung. In diesem Fall die wird die Eigenschaft **DisplayName** für die Identität zurückgegeben werden, aber die **Id**-Eigenschaft ist aus der Ressource nicht vorhanden.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity",
  "suppressions": [
    "Error: /api-reference/beta/resources/identity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
