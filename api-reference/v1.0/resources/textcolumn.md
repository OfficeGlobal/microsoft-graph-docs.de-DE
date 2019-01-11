---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: d064253cfad141d5879afb52451ca28fa2aeca67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860879"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="e82a1-102">TableColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e82a1-102">TextColumn resource type</span></span>

<span data-ttu-id="e82a1-103">Die **textColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Text handelt.</span><span class="sxs-lookup"><span data-stu-id="e82a1-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e82a1-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e82a1-104">JSON representation</span></span>

<span data-ttu-id="e82a1-105">Es folgt eine JSON-Darstellung einer **textColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="e82a1-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="e82a1-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e82a1-106">Properties</span></span>

| <span data-ttu-id="e82a1-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="e82a1-107">Property name</span></span>                   | <span data-ttu-id="e82a1-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e82a1-108">Type</span></span>    | <span data-ttu-id="e82a1-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e82a1-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="e82a1-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="e82a1-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="e82a1-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="e82a1-111">boolean</span></span> | <span data-ttu-id="e82a1-112">Gibt an, ob mehrere Textzeilen zugelassen sind.</span><span class="sxs-lookup"><span data-stu-id="e82a1-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="e82a1-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="e82a1-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="e82a1-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e82a1-114">boolean</span></span> | <span data-ttu-id="e82a1-115">Gibt an, ob Updates für diese Spalte den vorhandenen Text ersetzen oder an den vorhandenen Text angefügt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e82a1-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="e82a1-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="e82a1-116">**linesForEditing**</span></span>             | <span data-ttu-id="e82a1-117">int32</span><span class="sxs-lookup"><span data-stu-id="e82a1-117">int32</span></span>   | <span data-ttu-id="e82a1-118">Die Größe des Textfeldes.</span><span class="sxs-lookup"><span data-stu-id="e82a1-118">The size of the text box.</span></span>
| <span data-ttu-id="e82a1-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="e82a1-119">**maxLength**</span></span>                   | <span data-ttu-id="e82a1-120">int32</span><span class="sxs-lookup"><span data-stu-id="e82a1-120">int32</span></span>   | <span data-ttu-id="e82a1-121">Die maximal Anzahl Zeichen für den Wert.</span><span class="sxs-lookup"><span data-stu-id="e82a1-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="e82a1-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="e82a1-122">**textType**</span></span>                    | <span data-ttu-id="e82a1-123">string</span><span class="sxs-lookup"><span data-stu-id="e82a1-123">string</span></span>  | <span data-ttu-id="e82a1-124">Der Texttyp des gespeicherten Textes.</span><span class="sxs-lookup"><span data-stu-id="e82a1-124">The type of text being stored.</span></span> <span data-ttu-id="e82a1-125">Muss `plain` oder `richText` sein.</span><span class="sxs-lookup"><span data-stu-id="e82a1-125">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/textcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(plain,richText) are in resource, but () are in table"
  ],
  "tocPath": "Resources/TextColumn"
} -->
