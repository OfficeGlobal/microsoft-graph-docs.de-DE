---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 810554620e747d3160a6d8c74913518b8590c19d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019286"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="8881c-102">TableColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8881c-102">TextColumn resource type</span></span>

<span data-ttu-id="8881c-103">Die **textColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Text handelt.</span><span class="sxs-lookup"><span data-stu-id="8881c-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8881c-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8881c-104">JSON representation</span></span>

<span data-ttu-id="8881c-105">Es folgt eine JSON-Darstellung einer **textColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="8881c-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="8881c-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8881c-106">Properties</span></span>

| <span data-ttu-id="8881c-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="8881c-107">Property name</span></span>                   | <span data-ttu-id="8881c-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8881c-108">Type</span></span>    | <span data-ttu-id="8881c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8881c-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="8881c-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="8881c-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="8881c-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="8881c-111">boolean</span></span> | <span data-ttu-id="8881c-112">Gibt an, ob mehrere Textzeilen zugelassen sind.</span><span class="sxs-lookup"><span data-stu-id="8881c-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="8881c-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="8881c-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="8881c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8881c-114">boolean</span></span> | <span data-ttu-id="8881c-115">Gibt an, ob Updates für diese Spalte den vorhandenen Text ersetzen oder an den vorhandenen Text angefügt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8881c-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="8881c-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="8881c-116">**linesForEditing**</span></span>             | <span data-ttu-id="8881c-117">int32</span><span class="sxs-lookup"><span data-stu-id="8881c-117">int32</span></span>   | <span data-ttu-id="8881c-118">Die Größe des Textfeldes.</span><span class="sxs-lookup"><span data-stu-id="8881c-118">The size of the text box.</span></span>
| <span data-ttu-id="8881c-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="8881c-119">**maxLength**</span></span>                   | <span data-ttu-id="8881c-120">int32</span><span class="sxs-lookup"><span data-stu-id="8881c-120">int32</span></span>   | <span data-ttu-id="8881c-121">Die maximal Anzahl Zeichen für den Wert.</span><span class="sxs-lookup"><span data-stu-id="8881c-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="8881c-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="8881c-122">**textType**</span></span>                    | <span data-ttu-id="8881c-123">string</span><span class="sxs-lookup"><span data-stu-id="8881c-123">string</span></span>  | <span data-ttu-id="8881c-124">Der Texttyp des gespeicherten Textes.</span><span class="sxs-lookup"><span data-stu-id="8881c-124">The type of text being stored.</span></span> <span data-ttu-id="8881c-125">Muss `plain` oder `richText` sein.</span><span class="sxs-lookup"><span data-stu-id="8881c-125">Must be one of `plain` or `richText`</span></span>

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
