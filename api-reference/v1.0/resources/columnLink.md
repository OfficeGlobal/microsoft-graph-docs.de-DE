---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: 435696cc596f73830104ea8ec0619bf40a462d62
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834531"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="3c776-102">ColumnLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3c776-102">ColumnLink resource type</span></span>

<span data-ttu-id="3c776-103">A **ColumnLink** eines [ContentType][] fügt die Website **ColumnDefinition** zu diesem Inhaltstyp hinzu.</span><span class="sxs-lookup"><span data-stu-id="3c776-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="3c776-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c776-105">JSON representation</span></span>

<span data-ttu-id="3c776-106">Es folgt eine JSON-Darstellung einer **columnLink**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="3c776-106">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="3c776-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c776-107">Properties</span></span>

| <span data-ttu-id="3c776-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="3c776-108">Property name</span></span> | <span data-ttu-id="3c776-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3c776-109">Type</span></span>   | <span data-ttu-id="3c776-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c776-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="3c776-111">**id**</span><span class="sxs-lookup"><span data-stu-id="3c776-111">**id**</span></span>        | <span data-ttu-id="3c776-112">string</span><span class="sxs-lookup"><span data-stu-id="3c776-112">string</span></span> | <span data-ttu-id="3c776-113">Die eindeutige ID für die Spalte.</span><span class="sxs-lookup"><span data-stu-id="3c776-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="3c776-114">**name**</span><span class="sxs-lookup"><span data-stu-id="3c776-114">**name**</span></span>      | <span data-ttu-id="3c776-115">string</span><span class="sxs-lookup"><span data-stu-id="3c776-115">string</span></span> | <span data-ttu-id="3c776-116">Der Name der Spalte in diesem Inhaltstyp.</span><span class="sxs-lookup"><span data-stu-id="3c776-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
