---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 459e51af92e01d10edd2ec1d86f3c288b125e1d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957466"
---
# <a name="listinfo-resource"></a><span data-ttu-id="b7095-102">ListInfo-Ressource</span><span class="sxs-lookup"><span data-stu-id="b7095-102">ListInfo resource</span></span>

<span data-ttu-id="b7095-103">Der Komplexe Typ **listInfo** enthält zusätzliche Informationen zu einer [Liste][].</span><span class="sxs-lookup"><span data-stu-id="b7095-103">The **listInfo** complex type provides additional information about a [list][].</span></span>

[Liste]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="b7095-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b7095-105">JSON representation</span></span>

<span data-ttu-id="b7095-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b7095-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template": "documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a><span data-ttu-id="b7095-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b7095-107">Properties</span></span>

| <span data-ttu-id="b7095-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="b7095-108">Property name</span></span>           | <span data-ttu-id="b7095-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b7095-109">Type</span></span>    | <span data-ttu-id="b7095-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7095-110">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="b7095-111">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="b7095-111">**contentTypesEnabled**</span></span> | <span data-ttu-id="b7095-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7095-112">Boolean</span></span> | <span data-ttu-id="b7095-113">`true` gibt an, dass die Inhaltstypen für diese Liste aktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="b7095-113">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="b7095-114">**hidden**</span><span class="sxs-lookup"><span data-stu-id="b7095-114">**hidden**</span></span>              | <span data-ttu-id="b7095-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7095-115">Boolean</span></span> | <span data-ttu-id="b7095-116">`true` gibt an, dass die Liste normalerweise nicht in die SharePoint-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b7095-116">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="b7095-117">**template**</span><span class="sxs-lookup"><span data-stu-id="b7095-117">**template**</span></span>            | <span data-ttu-id="b7095-118">string</span><span class="sxs-lookup"><span data-stu-id="b7095-118">String</span></span>  | <span data-ttu-id="b7095-119">Ein Aufzählungswert, der die bei der Erstellung der Liste verwendete Basislistenvorlage verwendet.</span><span class="sxs-lookup"><span data-stu-id="b7095-119">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="b7095-120">Beispielwerte: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` etc.</span><span class="sxs-lookup"><span data-stu-id="b7095-120">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="b7095-121">Hinweise</span><span class="sxs-lookup"><span data-stu-id="b7095-121">Remarks</span></span>

<span data-ttu-id="b7095-122">Obgleich die meisten von Benutzern erstellen Listen einen der oben aufgeführten Werte enthalten, sind andere Werte ebenfalls möglich.</span><span class="sxs-lookup"><span data-stu-id="b7095-122">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="b7095-123">Ihre App sollte darauf vorbereitet werden, auch alle hier nicht aufgelisteten Werte zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="b7095-123">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="b7095-124">Hinweis für Entwickler, die mit CSOM-APIs von SharePoint vertraut sind: Der `template`-Wert entspricht der `SPListTemplateType`-Enumeration.</span><span class="sxs-lookup"><span data-stu-id="b7095-124">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/listinfo.md:
      Found potential enums in resource example that weren't defined in a table:(documentLibrary,genericList,tasks,survey,links,announcements,contacts,...) are in resource, but () are in table"
  ],
  "tocPath": ""
}-->
