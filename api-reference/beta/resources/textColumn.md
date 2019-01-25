---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 524f25b6b5097197daeb8b130b10ff7513010965
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525003"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="93c5e-102">TableColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="93c5e-102">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93c5e-103">Die **textColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Text handelt.</span><span class="sxs-lookup"><span data-stu-id="93c5e-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93c5e-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="93c5e-104">JSON representation</span></span>

<span data-ttu-id="93c5e-105">Es folgt eine JSON-Darstellung einer **textColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="93c5e-105">Here is a JSON representation of a **textColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a><span data-ttu-id="93c5e-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="93c5e-106">Properties</span></span>

| <span data-ttu-id="93c5e-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="93c5e-107">Property name</span></span>                   | <span data-ttu-id="93c5e-108">Typ</span><span class="sxs-lookup"><span data-stu-id="93c5e-108">Type</span></span>   | <span data-ttu-id="93c5e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93c5e-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="93c5e-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="93c5e-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="93c5e-111">string</span><span class="sxs-lookup"><span data-stu-id="93c5e-111">string</span></span> | <span data-ttu-id="93c5e-112">Gibt an, ob mehrere Textzeilen zugelassen sind.</span><span class="sxs-lookup"><span data-stu-id="93c5e-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="93c5e-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="93c5e-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="93c5e-114">string</span><span class="sxs-lookup"><span data-stu-id="93c5e-114">string</span></span> | <span data-ttu-id="93c5e-115">Gibt an, ob Updates für diese Spalte den vorhandenen Text ersetzen oder an den vorhandenen Text angefügt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="93c5e-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="93c5e-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="93c5e-116">**linesForEditing**</span></span>             | <span data-ttu-id="93c5e-117">int</span><span class="sxs-lookup"><span data-stu-id="93c5e-117">int</span></span>    | <span data-ttu-id="93c5e-118">Die Größe des Textfeldes.</span><span class="sxs-lookup"><span data-stu-id="93c5e-118">The size of the text box.</span></span>
| <span data-ttu-id="93c5e-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="93c5e-119">**maxLength**</span></span>                   | <span data-ttu-id="93c5e-120">int</span><span class="sxs-lookup"><span data-stu-id="93c5e-120">int</span></span>    | <span data-ttu-id="93c5e-121">Die maximal Anzahl Zeichen für den Wert.</span><span class="sxs-lookup"><span data-stu-id="93c5e-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="93c5e-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="93c5e-122">**textType**</span></span>                    | <span data-ttu-id="93c5e-123">string</span><span class="sxs-lookup"><span data-stu-id="93c5e-123">string</span></span> | <span data-ttu-id="93c5e-124">Der Texttyp des gespeicherten Textes.</span><span class="sxs-lookup"><span data-stu-id="93c5e-124">The type of text being stored.</span></span> <span data-ttu-id="93c5e-125">Muss `plain` oder `richText` sein.</span><span class="sxs-lookup"><span data-stu-id="93c5e-125">Must be one of `plain` or `richText`</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/textColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
