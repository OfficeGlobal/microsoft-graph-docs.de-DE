---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: 9feb49fc9c581a4518f63a0367087d54de32cff4
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264070"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="dea7d-102">ChoiceColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dea7d-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="dea7d-103">Die **ChoiceColumn** einer [ColumnDefinition](columnDefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer Auswahlliste ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="dea7d-103">The **choiceColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dea7d-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dea7d-104">JSON representation</span></span>

<span data-ttu-id="dea7d-105">Es folgt eine JSON-Darstellung einer **choiceColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="dea7d-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="dea7d-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dea7d-106">Properties</span></span>

| <span data-ttu-id="dea7d-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="dea7d-107">Property name</span></span>      | <span data-ttu-id="dea7d-108">Typ</span><span class="sxs-lookup"><span data-stu-id="dea7d-108">Type</span></span>               | <span data-ttu-id="dea7d-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dea7d-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="dea7d-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="dea7d-110">**allowTextEntry**</span></span> | <span data-ttu-id="dea7d-111">boolean</span><span class="sxs-lookup"><span data-stu-id="dea7d-111">boolean</span></span>            | <span data-ttu-id="dea7d-112">Ist der Wert true, sind benutzerdefinierte Werte, die sich nicht in der konfigurierten Auswahl befinden, zugelassen.</span><span class="sxs-lookup"><span data-stu-id="dea7d-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="dea7d-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="dea7d-113">**choices**</span></span>        | <span data-ttu-id="dea7d-114">Collection(string)</span><span class="sxs-lookup"><span data-stu-id="dea7d-114">collection(string)</span></span> | <span data-ttu-id="dea7d-115">Die Liste der Werte, die für diese Spalte zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="dea7d-115">The list of values available for this column.</span></span>
| <span data-ttu-id="dea7d-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="dea7d-116">**displayAs**</span></span>      | <span data-ttu-id="dea7d-117">string</span><span class="sxs-lookup"><span data-stu-id="dea7d-117">string</span></span>             | <span data-ttu-id="dea7d-118">Wie werden die Auswahlmöglichkeiten in der UX dargestellt?</span><span class="sxs-lookup"><span data-stu-id="dea7d-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="dea7d-119">Muss `checkBoxes`, `dropDownMenu` oder `radioButtons` sein.</span><span class="sxs-lookup"><span data-stu-id="dea7d-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ChoiceColumn"
} -->
