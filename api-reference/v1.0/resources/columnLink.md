---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: cdae360afb6e626ee481a7e98ed5f90e657203b2
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265120"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="b2da9-102">ColumnLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b2da9-102">ColumnLink resource type</span></span>

<span data-ttu-id="b2da9-103">A **ColumnLink** eines [ContentType][] fügt die Website **ColumnDefinition** zu diesem Inhaltstyp hinzu.</span><span class="sxs-lookup"><span data-stu-id="b2da9-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contentType.md

## <a name="json-representation"></a><span data-ttu-id="b2da9-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b2da9-105">JSON representation</span></span>

<span data-ttu-id="b2da9-106">Es folgt eine JSON-Darstellung einer **columnLink**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="b2da9-106">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="b2da9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b2da9-107">Properties</span></span>

| <span data-ttu-id="b2da9-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="b2da9-108">Property name</span></span> | <span data-ttu-id="b2da9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b2da9-109">Type</span></span>   | <span data-ttu-id="b2da9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2da9-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="b2da9-111">**ID**</span><span class="sxs-lookup"><span data-stu-id="b2da9-111">**id**</span></span>        | <span data-ttu-id="b2da9-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2da9-112">string</span></span> | <span data-ttu-id="b2da9-113">Die eindeutige ID für die Spalte.</span><span class="sxs-lookup"><span data-stu-id="b2da9-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="b2da9-114">**name**</span><span class="sxs-lookup"><span data-stu-id="b2da9-114">**name**</span></span>      | <span data-ttu-id="b2da9-115">string</span><span class="sxs-lookup"><span data-stu-id="b2da9-115">string</span></span> | <span data-ttu-id="b2da9-116">Der Name der Spalte in diesem Inhaltstyp.</span><span class="sxs-lookup"><span data-stu-id="b2da9-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
