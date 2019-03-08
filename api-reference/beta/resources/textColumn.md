---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: c69dc7c30bff0f43327ec256af6071e34de6b898
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481496"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="b3ec3-102">TableColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b3ec3-102">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3ec3-103">Die **textColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Text handelt.</span><span class="sxs-lookup"><span data-stu-id="b3ec3-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3ec3-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b3ec3-104">JSON representation</span></span>

<span data-ttu-id="b3ec3-105">Es folgt eine JSON-Darstellung einer **textColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="b3ec3-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="b3ec3-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b3ec3-106">Properties</span></span>

| <span data-ttu-id="b3ec3-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="b3ec3-107">Property name</span></span>                   | <span data-ttu-id="b3ec3-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b3ec3-108">Type</span></span>   | <span data-ttu-id="b3ec3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3ec3-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="b3ec3-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="b3ec3-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="b3ec3-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3ec3-111">string</span></span> | <span data-ttu-id="b3ec3-112">Gibt an, ob mehrere Textzeilen zugelassen sind.</span><span class="sxs-lookup"><span data-stu-id="b3ec3-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="b3ec3-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="b3ec3-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="b3ec3-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3ec3-114">string</span></span> | <span data-ttu-id="b3ec3-115">Gibt an, ob Updates für diese Spalte den vorhandenen Text ersetzen oder an den vorhandenen Text angefügt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b3ec3-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="b3ec3-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="b3ec3-116">**linesForEditing**</span></span>             | <span data-ttu-id="b3ec3-117">int</span><span class="sxs-lookup"><span data-stu-id="b3ec3-117">int</span></span>    | <span data-ttu-id="b3ec3-118">Die Größe des Textfeldes.</span><span class="sxs-lookup"><span data-stu-id="b3ec3-118">The size of the text box.</span></span>
| <span data-ttu-id="b3ec3-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="b3ec3-119">**maxLength**</span></span>                   | <span data-ttu-id="b3ec3-120">int</span><span class="sxs-lookup"><span data-stu-id="b3ec3-120">int</span></span>    | <span data-ttu-id="b3ec3-121">Die maximal Anzahl Zeichen für den Wert.</span><span class="sxs-lookup"><span data-stu-id="b3ec3-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="b3ec3-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="b3ec3-122">**textType**</span></span>                    | <span data-ttu-id="b3ec3-123">string</span><span class="sxs-lookup"><span data-stu-id="b3ec3-123">string</span></span> | <span data-ttu-id="b3ec3-124">Der Texttyp des gespeicherten Textes.</span><span class="sxs-lookup"><span data-stu-id="b3ec3-124">The type of text being stored.</span></span> <span data-ttu-id="b3ec3-125">Muss `plain` oder `richText` sein.</span><span class="sxs-lookup"><span data-stu-id="b3ec3-125">Must be one of `plain` or `richText`</span></span>

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
