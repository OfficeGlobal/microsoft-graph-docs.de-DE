---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.openlocfilehash: c1a29099264c46f32e09b375a97ff49c13c99c6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858457"
---
# <a name="listinfo-resource"></a><span data-ttu-id="eb6dc-102">ListInfo-Ressource</span><span class="sxs-lookup"><span data-stu-id="eb6dc-102">ListInfo resource</span></span>

> <span data-ttu-id="eb6dc-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eb6dc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb6dc-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eb6dc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb6dc-105">Der Komplexe Typ **listInfo** enthält zusätzliche Informationen zu einer [Liste][].</span><span class="sxs-lookup"><span data-stu-id="eb6dc-105">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="eb6dc-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eb6dc-107">JSON representation</span></span>

<span data-ttu-id="eb6dc-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eb6dc-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="eb6dc-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eb6dc-109">Properties</span></span>

| <span data-ttu-id="eb6dc-110">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="eb6dc-110">Property name</span></span>           | <span data-ttu-id="eb6dc-111">Typ</span><span class="sxs-lookup"><span data-stu-id="eb6dc-111">Type</span></span>    | <span data-ttu-id="eb6dc-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb6dc-112">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="eb6dc-113">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="eb6dc-113">**contentTypesEnabled**</span></span> | <span data-ttu-id="eb6dc-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb6dc-114">Boolean</span></span> | <span data-ttu-id="eb6dc-115">`true` gibt an, dass die Inhaltstypen für diese Liste aktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="eb6dc-115">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="eb6dc-116">**hidden**</span><span class="sxs-lookup"><span data-stu-id="eb6dc-116">**hidden**</span></span>              | <span data-ttu-id="eb6dc-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb6dc-117">Boolean</span></span> | <span data-ttu-id="eb6dc-118">`true` gibt an, dass die Liste normalerweise nicht in die SharePoint-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="eb6dc-118">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="eb6dc-119">**template**</span><span class="sxs-lookup"><span data-stu-id="eb6dc-119">**template**</span></span>            | <span data-ttu-id="eb6dc-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb6dc-120">String</span></span>  | <span data-ttu-id="eb6dc-121">Ein Aufzählungswert, der die bei der Erstellung der Liste verwendete Basislistenvorlage verwendet.</span><span class="sxs-lookup"><span data-stu-id="eb6dc-121">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="eb6dc-122">Beispielwerte: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` etc.</span><span class="sxs-lookup"><span data-stu-id="eb6dc-122">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="eb6dc-123">Hinweise</span><span class="sxs-lookup"><span data-stu-id="eb6dc-123">Remarks</span></span>

<span data-ttu-id="eb6dc-124">Obgleich die meisten von Benutzern erstellen Listen einen der oben aufgeführten Werte enthalten, sind andere Werte ebenfalls möglich.</span><span class="sxs-lookup"><span data-stu-id="eb6dc-124">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="eb6dc-125">Ihre App sollte darauf vorbereitet werden, auch alle hier nicht aufgelisteten Werte zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="eb6dc-125">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="eb6dc-126">Hinweis für Entwickler, die mit CSOM-APIs von SharePoint vertraut sind: Der `template`-Wert entspricht der `SPListTemplateType`-Enumeration.</span><span class="sxs-lookup"><span data-stu-id="eb6dc-126">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
