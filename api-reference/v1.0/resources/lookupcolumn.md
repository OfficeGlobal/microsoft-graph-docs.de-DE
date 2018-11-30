---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
ms.openlocfilehash: 73d372d52447906c826d79e3c614635a3023cefa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018641"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="68a50-102">LookupColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="68a50-102">LookupColumn resource type</span></span>

<span data-ttu-id="68a50-103">Die **lookupColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer anderen Quelle der Website nachgeschlagen werden.</span><span class="sxs-lookup"><span data-stu-id="68a50-103">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68a50-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="68a50-104">JSON representation</span></span>

<span data-ttu-id="68a50-105">Es folgt eine JSON-Darstellung einer **lookupColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="68a50-105">Here is a JSON representation of a **lookupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="68a50-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="68a50-106">Properties</span></span>

| <span data-ttu-id="68a50-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="68a50-107">Property name</span></span>             | <span data-ttu-id="68a50-108">Typ</span><span class="sxs-lookup"><span data-stu-id="68a50-108">Type</span></span>    | <span data-ttu-id="68a50-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68a50-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="68a50-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="68a50-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="68a50-111">boolean</span><span class="sxs-lookup"><span data-stu-id="68a50-111">boolean</span></span> | <span data-ttu-id="68a50-112">Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="68a50-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="68a50-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="68a50-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="68a50-114">boolean</span><span class="sxs-lookup"><span data-stu-id="68a50-114">boolean</span></span> | <span data-ttu-id="68a50-115">Gibt an, ob die Werte in der Spalte die standardmäßige Grenze von 255 Zeichen überschreiten dürfen.</span><span class="sxs-lookup"><span data-stu-id="68a50-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="68a50-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="68a50-116">**columnName**</span></span>            | <span data-ttu-id="68a50-117">string</span><span class="sxs-lookup"><span data-stu-id="68a50-117">string</span></span>  | <span data-ttu-id="68a50-118">Der Name der Nachschlagequellen-Spalte.</span><span class="sxs-lookup"><span data-stu-id="68a50-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="68a50-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="68a50-119">**listId**</span></span>                | <span data-ttu-id="68a50-120">string</span><span class="sxs-lookup"><span data-stu-id="68a50-120">string</span></span>  | <span data-ttu-id="68a50-121">Der eindeutige Bezeichner der Nachschlagequellen-Liste.</span><span class="sxs-lookup"><span data-stu-id="68a50-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="68a50-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="68a50-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="68a50-123">string</span><span class="sxs-lookup"><span data-stu-id="68a50-123">string</span></span>  | <span data-ttu-id="68a50-124">Wenn angegeben, erfolgt in dieser Spalte ein *zweites Nachschlagen*. In der Liste wird ein weiteres Feld zu dem beim *ersten Nachschlagen* ermittelten Element hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="68a50-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="68a50-125">Verwenden Sie das Listenelement des \*ersten \* Nachschlagens als Quelle für die hier genannte Spalte.</span><span class="sxs-lookup"><span data-stu-id="68a50-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
