---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 80e41b379b9b4ce51a3ee6c910447a22f43356c3
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="bb993-102">TableColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bb993-102">TextColumn resource type</span></span>

<span data-ttu-id="bb993-103">Die **textColumn** einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Text handelt.</span><span class="sxs-lookup"><span data-stu-id="bb993-103">The **textColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb993-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bb993-104">JSON representation</span></span>

<span data-ttu-id="bb993-105">Es folgt eine JSON-Darstellung einer **textColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="bb993-105">Here is a JSON representation of a **baseItem** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="bb993-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bb993-106">Properties</span></span>

| <span data-ttu-id="bb993-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="bb993-107">Property name</span></span>                   | <span data-ttu-id="bb993-108">Typ</span><span class="sxs-lookup"><span data-stu-id="bb993-108">Type</span></span>   | <span data-ttu-id="bb993-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb993-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="bb993-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="bb993-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="bb993-111">string</span><span class="sxs-lookup"><span data-stu-id="bb993-111">string</span></span> | <span data-ttu-id="bb993-112">Gibt an, ob mehrere Textzeilen zugelassen sind.</span><span class="sxs-lookup"><span data-stu-id="bb993-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="bb993-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="bb993-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="bb993-114">string</span><span class="sxs-lookup"><span data-stu-id="bb993-114">string</span></span> | <span data-ttu-id="bb993-115">Gibt an, ob Updates für diese Spalte den vorhandenen Text ersetzen oder an den vorhandenen Text angefügt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bb993-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="bb993-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="bb993-116">**linesForEditing**</span></span>             | <span data-ttu-id="bb993-117">int</span><span class="sxs-lookup"><span data-stu-id="bb993-117">int</span></span>    | <span data-ttu-id="bb993-118">Die Größe des Textfeldes.</span><span class="sxs-lookup"><span data-stu-id="bb993-118">The size of the text box.</span></span>
| <span data-ttu-id="bb993-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="bb993-119">**maxLength**</span></span>                   | <span data-ttu-id="bb993-120">int</span><span class="sxs-lookup"><span data-stu-id="bb993-120">int</span></span>    | <span data-ttu-id="bb993-121">Die maximal Anzahl Zeichen für den Wert.</span><span class="sxs-lookup"><span data-stu-id="bb993-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="bb993-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="bb993-122">**textType**</span></span>                    | <span data-ttu-id="bb993-123">string</span><span class="sxs-lookup"><span data-stu-id="bb993-123">string</span></span> | <span data-ttu-id="bb993-124">Der Texttyp des gespeicherten Textes.</span><span class="sxs-lookup"><span data-stu-id="bb993-124">The type of text being stored.</span></span> <span data-ttu-id="bb993-125">Muss `plain` oder `richText` sein.</span><span class="sxs-lookup"><span data-stu-id="bb993-125">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
