---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 5ff280b6c969d9832e2f81f77dc32237f9905aad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061636"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="16729-102">TableColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="16729-102">TextColumn resource type</span></span>

> <span data-ttu-id="16729-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="16729-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16729-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16729-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16729-105">Die **textColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Text handelt.</span><span class="sxs-lookup"><span data-stu-id="16729-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16729-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16729-106">JSON representation</span></span>

<span data-ttu-id="16729-107">Es folgt eine JSON-Darstellung einer **textColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="16729-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="16729-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16729-108">Properties</span></span>

| <span data-ttu-id="16729-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="16729-109">Property name</span></span>                   | <span data-ttu-id="16729-110">Typ</span><span class="sxs-lookup"><span data-stu-id="16729-110">Type</span></span>   | <span data-ttu-id="16729-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16729-111">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="16729-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="16729-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="16729-113">string</span><span class="sxs-lookup"><span data-stu-id="16729-113">string</span></span> | <span data-ttu-id="16729-114">Gibt an, ob mehrere Textzeilen zugelassen sind.</span><span class="sxs-lookup"><span data-stu-id="16729-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="16729-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="16729-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="16729-116">string</span><span class="sxs-lookup"><span data-stu-id="16729-116">string</span></span> | <span data-ttu-id="16729-117">Gibt an, ob Updates für diese Spalte den vorhandenen Text ersetzen oder an den vorhandenen Text angefügt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="16729-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="16729-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="16729-118">**linesForEditing**</span></span>             | <span data-ttu-id="16729-119">int</span><span class="sxs-lookup"><span data-stu-id="16729-119">int</span></span>    | <span data-ttu-id="16729-120">Die Größe des Textfeldes.</span><span class="sxs-lookup"><span data-stu-id="16729-120">The size of the text box.</span></span>
| <span data-ttu-id="16729-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="16729-121">**maxLength**</span></span>                   | <span data-ttu-id="16729-122">int</span><span class="sxs-lookup"><span data-stu-id="16729-122">int</span></span>    | <span data-ttu-id="16729-123">Die maximal Anzahl Zeichen für den Wert.</span><span class="sxs-lookup"><span data-stu-id="16729-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="16729-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="16729-124">**textType**</span></span>                    | <span data-ttu-id="16729-125">string</span><span class="sxs-lookup"><span data-stu-id="16729-125">string</span></span> | <span data-ttu-id="16729-126">Der Texttyp des gespeicherten Textes.</span><span class="sxs-lookup"><span data-stu-id="16729-126">The type of text being stored.</span></span> <span data-ttu-id="16729-127">Muss `plain` oder `richText` sein.</span><span class="sxs-lookup"><span data-stu-id="16729-127">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
