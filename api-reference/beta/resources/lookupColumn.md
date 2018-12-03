---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
ms.openlocfilehash: 92eb43dad2ceca173fba79ad7d40f51f488a992c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058207"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="4ba20-102">LookupColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4ba20-102">LookupColumn resource type</span></span>

> <span data-ttu-id="4ba20-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4ba20-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ba20-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4ba20-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ba20-105">Die **lookupColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer anderen Quelle der Website nachgeschlagen werden.</span><span class="sxs-lookup"><span data-stu-id="4ba20-105">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ba20-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4ba20-106">JSON representation</span></span>

<span data-ttu-id="4ba20-107">Es folgt eine JSON-Darstellung einer **lookupColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="4ba20-107">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="4ba20-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4ba20-108">Properties</span></span>

| <span data-ttu-id="4ba20-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="4ba20-109">Property name</span></span>             | <span data-ttu-id="4ba20-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4ba20-110">Type</span></span>    | <span data-ttu-id="4ba20-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ba20-111">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="4ba20-112">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="4ba20-112">**allowMultipleValues**</span></span>   | <span data-ttu-id="4ba20-113">boolean</span><span class="sxs-lookup"><span data-stu-id="4ba20-113">boolean</span></span> | <span data-ttu-id="4ba20-114">Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="4ba20-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="4ba20-115">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="4ba20-115">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="4ba20-116">boolean</span><span class="sxs-lookup"><span data-stu-id="4ba20-116">boolean</span></span> | <span data-ttu-id="4ba20-117">Gibt an, ob die Werte in der Spalte die standardmäßige Grenze von 255 Zeichen überschreiten dürfen.</span><span class="sxs-lookup"><span data-stu-id="4ba20-117">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="4ba20-118">**columnName**</span><span class="sxs-lookup"><span data-stu-id="4ba20-118">**columnName**</span></span>            | <span data-ttu-id="4ba20-119">string</span><span class="sxs-lookup"><span data-stu-id="4ba20-119">string</span></span>  | <span data-ttu-id="4ba20-120">Der Name der Nachschlagequellen-Spalte.</span><span class="sxs-lookup"><span data-stu-id="4ba20-120">The name of the lookup source column.</span></span>
| <span data-ttu-id="4ba20-121">**listId**</span><span class="sxs-lookup"><span data-stu-id="4ba20-121">**listId**</span></span>                | <span data-ttu-id="4ba20-122">string</span><span class="sxs-lookup"><span data-stu-id="4ba20-122">string</span></span>  | <span data-ttu-id="4ba20-123">Der eindeutige Bezeichner der Nachschlagequellen-Liste.</span><span class="sxs-lookup"><span data-stu-id="4ba20-123">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="4ba20-124">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="4ba20-124">**primaryLookupColumnId**</span></span> | <span data-ttu-id="4ba20-125">string</span><span class="sxs-lookup"><span data-stu-id="4ba20-125">string</span></span>  | <span data-ttu-id="4ba20-126">Wenn angegeben, erfolgt in dieser Spalte ein *zweites Nachschlagen*. In der Liste wird ein weiteres Feld zu dem beim *ersten Nachschlagen* ermittelten Element hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4ba20-126">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="4ba20-127">Verwenden Sie das Listenelement des \*ersten \* Nachschlagens als Quelle für die hier genannte Spalte.</span><span class="sxs-lookup"><span data-stu-id="4ba20-127">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
