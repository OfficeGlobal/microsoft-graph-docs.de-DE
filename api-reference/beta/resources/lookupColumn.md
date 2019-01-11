---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: 1c7ab364777e1e3f82bb78d8e0940cf4f85576a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885708"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="7ad6a-102">LookupColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7ad6a-102">LookupColumn resource type</span></span>

> <span data-ttu-id="7ad6a-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7ad6a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ad6a-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ad6a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ad6a-105">Die **lookupColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer anderen Quelle der Website nachgeschlagen werden.</span><span class="sxs-lookup"><span data-stu-id="7ad6a-105">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ad6a-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7ad6a-106">JSON representation</span></span>

<span data-ttu-id="7ad6a-107">Es folgt eine JSON-Darstellung einer **lookupColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="7ad6a-107">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="7ad6a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7ad6a-108">Properties</span></span>

| <span data-ttu-id="7ad6a-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="7ad6a-109">Property name</span></span>             | <span data-ttu-id="7ad6a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7ad6a-110">Type</span></span>    | <span data-ttu-id="7ad6a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ad6a-111">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="7ad6a-112">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="7ad6a-112">**allowMultipleValues**</span></span>   | <span data-ttu-id="7ad6a-113">boolean</span><span class="sxs-lookup"><span data-stu-id="7ad6a-113">boolean</span></span> | <span data-ttu-id="7ad6a-114">Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="7ad6a-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="7ad6a-115">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="7ad6a-115">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="7ad6a-116">boolean</span><span class="sxs-lookup"><span data-stu-id="7ad6a-116">boolean</span></span> | <span data-ttu-id="7ad6a-117">Gibt an, ob die Werte in der Spalte die standardmäßige Grenze von 255 Zeichen überschreiten dürfen.</span><span class="sxs-lookup"><span data-stu-id="7ad6a-117">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="7ad6a-118">**columnName**</span><span class="sxs-lookup"><span data-stu-id="7ad6a-118">**columnName**</span></span>            | <span data-ttu-id="7ad6a-119">string</span><span class="sxs-lookup"><span data-stu-id="7ad6a-119">string</span></span>  | <span data-ttu-id="7ad6a-120">Der Name der Nachschlagequellen-Spalte.</span><span class="sxs-lookup"><span data-stu-id="7ad6a-120">The name of the lookup source column.</span></span>
| <span data-ttu-id="7ad6a-121">**listId**</span><span class="sxs-lookup"><span data-stu-id="7ad6a-121">**listId**</span></span>                | <span data-ttu-id="7ad6a-122">string</span><span class="sxs-lookup"><span data-stu-id="7ad6a-122">string</span></span>  | <span data-ttu-id="7ad6a-123">Der eindeutige Bezeichner der Nachschlagequellen-Liste.</span><span class="sxs-lookup"><span data-stu-id="7ad6a-123">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="7ad6a-124">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="7ad6a-124">**primaryLookupColumnId**</span></span> | <span data-ttu-id="7ad6a-125">string</span><span class="sxs-lookup"><span data-stu-id="7ad6a-125">string</span></span>  | <span data-ttu-id="7ad6a-126">Wenn angegeben, erfolgt in dieser Spalte ein *zweites Nachschlagen*. In der Liste wird ein weiteres Feld zu dem beim *ersten Nachschlagen* ermittelten Element hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="7ad6a-126">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="7ad6a-127">Verwenden Sie das Listenelement des \*ersten \* Nachschlagens als Quelle für die hier genannte Spalte.</span><span class="sxs-lookup"><span data-stu-id="7ad6a-127">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
