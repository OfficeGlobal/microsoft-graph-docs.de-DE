---
title: plannerExternalReferences-Ressourcentyp
description: Die **plannerExternalReferences**-Ressource stellt die Sammlung der Verweise für eine Aufgabe dar. Es handelt sich um einen offenen Typ. Sie ist Bestandteil des taskDetails-Objekts. Der Wert im Eigenschaft-Wert-Paar ist das externalReference-Objekt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 23ebd270bd97455ad09d67870c5fbb8fc37cd051
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516287"
---
# <a name="plannerexternalreferences-resource-type"></a>plannerExternalReferences-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **plannerExternalReferences**-Ressource stellt die Sammlung der Verweise für eine Aufgabe dar. Es handelt sich um einen offenen Typ. Sie ist Bestandteil des [taskDetails](plannertaskdetails.md)-Objekts. Der Wert im Eigenschaft-Wert-Paar ist das [externalReference](plannerexternalreference.md)-Objekt.


## <a name="properties"></a>Eigenschaften
Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client **gültige URLs** auf Basis der Protokolle **HTTP/HTTPS** als Eigenschaften angeben, und ihre Werte müssen die [externalReference](plannerexternalreference.md)-Objekte sein. Basierend auf OData dürfen Eigenschaftennamen in offenen Typen die folgenden Zeichen nicht enthalten: `.`, `:`, `%`; daher müssen sie codiert werden. Nachfolgend ein Beispiel. Um einen Verweis zu entfernen, legen Sie den Wert der Eigenschaft auf `null` fest.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReferences"
}-->


```json
{
  "String-value":
  {
    "alias": "String-value",
    "lastModifiedBy": "String-value",
    "lastModifiedDateTime": "String(timestamp)",
    "previewPriority": "String-value",
    "type": "String-value"
  }
}
```

// Beispiel

```json
{
  "https%3A//contoso%2Esharepoint%2Ecom/teams/agile/documents/AnnualReport%2Epptx":
  {
    "@odata.type": "microsoft.graph.externalReference", // required in PATCH requests to edit the references on a task
    "alias": "Agile Team Annual Report",
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedDateTime": "2015-09-21T17:45:12.039Z",
    "previewPriority": "0009005756397228702",
    "type": "PowerPoint"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerexternalreferences.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
