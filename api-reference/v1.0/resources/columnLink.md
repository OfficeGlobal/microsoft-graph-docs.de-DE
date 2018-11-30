---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: a3eae28dcd9fef3ddfba9b39103bec31ff71c9da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016076"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="3f62f-102">ColumnLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3f62f-102">ColumnLink resource type</span></span>

<span data-ttu-id="3f62f-103">A **ColumnLink** eines [ContentType][] fügt die Website **ColumnDefinition** zu diesem Inhaltstyp hinzu.</span><span class="sxs-lookup"><span data-stu-id="3f62f-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="3f62f-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3f62f-105">JSON representation</span></span>

<span data-ttu-id="3f62f-106">Es folgt eine JSON-Darstellung einer **columnLink**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="3f62f-106">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="3f62f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3f62f-107">Properties</span></span>

| <span data-ttu-id="3f62f-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="3f62f-108">Property name</span></span> | <span data-ttu-id="3f62f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3f62f-109">Type</span></span>   | <span data-ttu-id="3f62f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3f62f-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="3f62f-111">**id**</span><span class="sxs-lookup"><span data-stu-id="3f62f-111">**id**</span></span>        | <span data-ttu-id="3f62f-112">string</span><span class="sxs-lookup"><span data-stu-id="3f62f-112">string</span></span> | <span data-ttu-id="3f62f-113">Die eindeutige ID für die Spalte.</span><span class="sxs-lookup"><span data-stu-id="3f62f-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="3f62f-114">**name**</span><span class="sxs-lookup"><span data-stu-id="3f62f-114">**name**</span></span>      | <span data-ttu-id="3f62f-115">string</span><span class="sxs-lookup"><span data-stu-id="3f62f-115">string</span></span> | <span data-ttu-id="3f62f-116">Der Name der Spalte in diesem Inhaltstyp.</span><span class="sxs-lookup"><span data-stu-id="3f62f-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
