---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: b5c41091b9193aabc36ee04e9dcc310bfc110af1
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264287"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="0fe29-102">TableColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0fe29-102">TextColumn resource type</span></span>

<span data-ttu-id="0fe29-103">Die **textColumn** einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Text handelt.</span><span class="sxs-lookup"><span data-stu-id="0fe29-103">The **textColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fe29-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0fe29-104">JSON representation</span></span>

<span data-ttu-id="0fe29-105">Es folgt eine JSON-Darstellung einer **textColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="0fe29-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="0fe29-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0fe29-106">Properties</span></span>

| <span data-ttu-id="0fe29-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="0fe29-107">Property name</span></span>                   | <span data-ttu-id="0fe29-108">Typ</span><span class="sxs-lookup"><span data-stu-id="0fe29-108">Type</span></span>    | <span data-ttu-id="0fe29-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fe29-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="0fe29-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="0fe29-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="0fe29-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0fe29-111">boolean</span></span> | <span data-ttu-id="0fe29-112">Gibt an, ob mehrere Textzeilen zugelassen sind.</span><span class="sxs-lookup"><span data-stu-id="0fe29-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="0fe29-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="0fe29-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="0fe29-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0fe29-114">boolean</span></span> | <span data-ttu-id="0fe29-115">Gibt an, ob Updates für diese Spalte den vorhandenen Text ersetzen oder an den vorhandenen Text angefügt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0fe29-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="0fe29-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="0fe29-116">**linesForEditing**</span></span>             | <span data-ttu-id="0fe29-117">Int32</span><span class="sxs-lookup"><span data-stu-id="0fe29-117">int32</span></span>   | <span data-ttu-id="0fe29-118">Die Größe des Textfeldes.</span><span class="sxs-lookup"><span data-stu-id="0fe29-118">The size of the text box.</span></span>
| <span data-ttu-id="0fe29-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="0fe29-119">**maxLength**</span></span>                   | <span data-ttu-id="0fe29-120">Int32</span><span class="sxs-lookup"><span data-stu-id="0fe29-120">int32</span></span>   | <span data-ttu-id="0fe29-121">Die maximal Anzahl Zeichen für den Wert.</span><span class="sxs-lookup"><span data-stu-id="0fe29-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="0fe29-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="0fe29-122">**textType**</span></span>                    | <span data-ttu-id="0fe29-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fe29-123">string</span></span>  | <span data-ttu-id="0fe29-124">Der Texttyp des gespeicherten Textes.</span><span class="sxs-lookup"><span data-stu-id="0fe29-124">The type of text being stored.</span></span> <span data-ttu-id="0fe29-125">Muss `plain` oder `richText` sein. `richText`</span><span class="sxs-lookup"><span data-stu-id="0fe29-125">Must be one of `plain` or `richText`</span></span>

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
