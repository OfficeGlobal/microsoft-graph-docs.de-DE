---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: dbb2fe0f651a269d69b880d18748b27a5b6f457c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480355"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="bd3e5-102">LookupColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bd3e5-102">LookupColumn resource type</span></span>

<span data-ttu-id="bd3e5-103">Die **lookupColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer anderen Quelle der Website nachgeschlagen werden.</span><span class="sxs-lookup"><span data-stu-id="bd3e5-103">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd3e5-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd3e5-104">JSON representation</span></span>

<span data-ttu-id="bd3e5-105">Es folgt eine JSON-Darstellung einer **lookupColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd3e5-105">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="bd3e5-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd3e5-106">Properties</span></span>

| <span data-ttu-id="bd3e5-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="bd3e5-107">Property name</span></span>             | <span data-ttu-id="bd3e5-108">Typ</span><span class="sxs-lookup"><span data-stu-id="bd3e5-108">Type</span></span>    | <span data-ttu-id="bd3e5-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd3e5-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="bd3e5-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="bd3e5-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="bd3e5-111">Boolesch</span><span class="sxs-lookup"><span data-stu-id="bd3e5-111">boolean</span></span> | <span data-ttu-id="bd3e5-112">Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="bd3e5-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="bd3e5-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="bd3e5-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="bd3e5-114">boolean</span><span class="sxs-lookup"><span data-stu-id="bd3e5-114">boolean</span></span> | <span data-ttu-id="bd3e5-115">Gibt an, ob die Werte in der Spalte die standardmäßige Grenze von 255 Zeichen überschreiten dürfen.</span><span class="sxs-lookup"><span data-stu-id="bd3e5-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="bd3e5-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="bd3e5-116">**columnName**</span></span>            | <span data-ttu-id="bd3e5-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd3e5-117">string</span></span>  | <span data-ttu-id="bd3e5-118">Der Name der Nachschlagequellen-Spalte.</span><span class="sxs-lookup"><span data-stu-id="bd3e5-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="bd3e5-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="bd3e5-119">**listId**</span></span>                | <span data-ttu-id="bd3e5-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd3e5-120">string</span></span>  | <span data-ttu-id="bd3e5-121">Der eindeutige Bezeichner der Nachschlagequellen-Liste.</span><span class="sxs-lookup"><span data-stu-id="bd3e5-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="bd3e5-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="bd3e5-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="bd3e5-123">string</span><span class="sxs-lookup"><span data-stu-id="bd3e5-123">string</span></span>  | <span data-ttu-id="bd3e5-124">Wenn angegeben, erfolgt in dieser Spalte ein *zweites Nachschlagen*. In der Liste wird ein weiteres Feld zu dem beim *ersten Nachschlagen* ermittelten Element hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="bd3e5-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="bd3e5-125">Verwenden Sie das Listenelement des \*ersten \* Nachschlagens als Quelle für die hier genannte Spalte.</span><span class="sxs-lookup"><span data-stu-id="bd3e5-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
