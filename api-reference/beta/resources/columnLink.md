---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: d5b1d068202057bc6a07982d04ff77b6bf07f028
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511863"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="32654-102">ColumnLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="32654-102">ColumnLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32654-103">A **ColumnLink** eines [ContentType][] fügt die Website **ColumnDefinition** zu diesem Inhaltstyp hinzu.</span><span class="sxs-lookup"><span data-stu-id="32654-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="32654-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="32654-105">JSON representation</span></span>

<span data-ttu-id="32654-106">Es folgt eine JSON-Darstellung einer **columnLink**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="32654-106">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="32654-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="32654-107">Properties</span></span>

| <span data-ttu-id="32654-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="32654-108">Property name</span></span> | <span data-ttu-id="32654-109">Typ</span><span class="sxs-lookup"><span data-stu-id="32654-109">Type</span></span>   | <span data-ttu-id="32654-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32654-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="32654-111">**id**</span><span class="sxs-lookup"><span data-stu-id="32654-111">**id**</span></span>        | <span data-ttu-id="32654-112">string</span><span class="sxs-lookup"><span data-stu-id="32654-112">string</span></span> | <span data-ttu-id="32654-113">Die eindeutige ID für die Spalte.</span><span class="sxs-lookup"><span data-stu-id="32654-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="32654-114">**name**</span><span class="sxs-lookup"><span data-stu-id="32654-114">**name**</span></span>      | <span data-ttu-id="32654-115">string</span><span class="sxs-lookup"><span data-stu-id="32654-115">string</span></span> | <span data-ttu-id="32654-116">Der Name der Spalte in diesem Inhaltstyp.</span><span class="sxs-lookup"><span data-stu-id="32654-116">The name of the column  in this content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": [
    "Error: /api-reference/beta/resources/columnLink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
