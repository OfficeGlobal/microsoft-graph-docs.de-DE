---
title: plannerExternalReferences-Ressourcentyp
description: Die **plannerExternalReferences**-Ressource stellt die Sammlung der Verweise für eine Aufgabe dar. Es handelt sich um einen offenen Typ. Sie ist Bestandteil des taskDetails-Objekts. Der Wert im Eigenschaft-Wert-Paar ist das externalReference-Objekt.
localization_priority: Normal
ms.openlocfilehash: aedfd0321843c4a906defe22f184bac7d293a6e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862076"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="1b093-106">plannerExternalReferences-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1b093-106">plannerExternalReferences resource type</span></span>

<span data-ttu-id="1b093-p102">Die **plannerExternalReferences**-Ressource stellt die Sammlung der Verweise für eine Aufgabe dar. Es handelt sich um einen offenen Typ. Sie ist Bestandteil des [taskDetails](plannertaskdetails.md)-Objekts. Der Wert im Eigenschaft-Wert-Paar ist das [externalReference](plannerexternalreference.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="1b093-p102">The **plannerExternalReferences** resource represents the collection of references on a task. This is an Open Type. It is part of the [task details](plannertaskdetails.md) object. The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="1b093-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1b093-111">Properties</span></span>
<span data-ttu-id="1b093-p103">Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client **gültige URLs** auf Basis der Protokolle **HTTP/HTTPS** als Eigenschaften angeben, und ihre Werte müssen die [externalReference](plannerexternalreference.md)-Objekte sein. Basierend auf OData dürfen Eigenschaftennamen in offenen Typen die folgenden Zeichen nicht enthalten: `.`, `:`, `%`; daher müssen sie codiert werden. Nachfolgend ein Beispiel. Um einen Verweis zu entfernen, legen Sie den Wert der Eigenschaft auf `null` fest.</span><span class="sxs-lookup"><span data-stu-id="1b093-p103">Properties of an Open Type can be defined by the client. In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects. Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded. Example is shown below. To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b093-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1b093-117">JSON representation</span></span>

<span data-ttu-id="1b093-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1b093-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
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

<span data-ttu-id="1b093-119">// Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b093-119">// Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
