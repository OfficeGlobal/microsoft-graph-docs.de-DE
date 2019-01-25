---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: 2efb199fafbf7c60af0e13720ea1b9efd93dc05c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517519"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="f9bab-102">LookupColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f9bab-102">LookupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9bab-103">Die **lookupColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer anderen Quelle der Website nachgeschlagen werden.</span><span class="sxs-lookup"><span data-stu-id="f9bab-103">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9bab-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f9bab-104">JSON representation</span></span>

<span data-ttu-id="f9bab-105">Es folgt eine JSON-Darstellung einer **lookupColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9bab-105">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="f9bab-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f9bab-106">Properties</span></span>

| <span data-ttu-id="f9bab-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="f9bab-107">Property name</span></span>             | <span data-ttu-id="f9bab-108">Typ</span><span class="sxs-lookup"><span data-stu-id="f9bab-108">Type</span></span>    | <span data-ttu-id="f9bab-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9bab-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="f9bab-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="f9bab-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="f9bab-111">boolean</span><span class="sxs-lookup"><span data-stu-id="f9bab-111">boolean</span></span> | <span data-ttu-id="f9bab-112">Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="f9bab-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="f9bab-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="f9bab-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="f9bab-114">boolean</span><span class="sxs-lookup"><span data-stu-id="f9bab-114">boolean</span></span> | <span data-ttu-id="f9bab-115">Gibt an, ob die Werte in der Spalte die standardmäßige Grenze von 255 Zeichen überschreiten dürfen.</span><span class="sxs-lookup"><span data-stu-id="f9bab-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="f9bab-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="f9bab-116">**columnName**</span></span>            | <span data-ttu-id="f9bab-117">string</span><span class="sxs-lookup"><span data-stu-id="f9bab-117">string</span></span>  | <span data-ttu-id="f9bab-118">Der Name der Nachschlagequellen-Spalte.</span><span class="sxs-lookup"><span data-stu-id="f9bab-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="f9bab-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="f9bab-119">**listId**</span></span>                | <span data-ttu-id="f9bab-120">string</span><span class="sxs-lookup"><span data-stu-id="f9bab-120">string</span></span>  | <span data-ttu-id="f9bab-121">Der eindeutige Bezeichner der Nachschlagequellen-Liste.</span><span class="sxs-lookup"><span data-stu-id="f9bab-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="f9bab-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="f9bab-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="f9bab-123">string</span><span class="sxs-lookup"><span data-stu-id="f9bab-123">string</span></span>  | <span data-ttu-id="f9bab-124">Wenn angegeben, erfolgt in dieser Spalte ein *zweites Nachschlagen*. In der Liste wird ein weiteres Feld zu dem beim *ersten Nachschlagen* ermittelten Element hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f9bab-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="f9bab-125">Verwenden Sie das Listenelement des \*ersten \* Nachschlagens als Quelle für die hier genannte Spalte.</span><span class="sxs-lookup"><span data-stu-id="f9bab-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/lookupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
