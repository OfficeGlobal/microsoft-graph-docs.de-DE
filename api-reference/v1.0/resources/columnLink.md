---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: ef7fef6fb6ca35f1117433b452de0841691282a0
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="a2a75-102">ColumnLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a2a75-102">ColumnLink resource type</span></span>

<span data-ttu-id="a2a75-103">A **ColumnLink** eines [ContentType][] fügt die Website **ColumnDefinition** zu diesem Inhaltstyp hinzu.</span><span class="sxs-lookup"><span data-stu-id="a2a75-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contentType.md

## <a name="json-representation"></a><span data-ttu-id="a2a75-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a2a75-105">JSON representation</span></span>

<span data-ttu-id="a2a75-106">Es folgt eine JSON-Darstellung einer **columnLink**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="a2a75-106">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="a2a75-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a2a75-107">Properties</span></span>

| <span data-ttu-id="a2a75-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="a2a75-108">Property name</span></span> | <span data-ttu-id="a2a75-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a2a75-109">Type</span></span>   | <span data-ttu-id="a2a75-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2a75-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a2a75-111">**id**</span><span class="sxs-lookup"><span data-stu-id="a2a75-111">**id**</span></span>        | <span data-ttu-id="a2a75-112">string</span><span class="sxs-lookup"><span data-stu-id="a2a75-112">string</span></span> | <span data-ttu-id="a2a75-113">Die eindeutige ID für die Spalte.</span><span class="sxs-lookup"><span data-stu-id="a2a75-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="a2a75-114">**name**</span><span class="sxs-lookup"><span data-stu-id="a2a75-114">**name**</span></span>      | <span data-ttu-id="a2a75-115">string</span><span class="sxs-lookup"><span data-stu-id="a2a75-115">string</span></span> | <span data-ttu-id="a2a75-116">Der Name der Spalte in diesem Inhaltstyp.</span><span class="sxs-lookup"><span data-stu-id="a2a75-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
