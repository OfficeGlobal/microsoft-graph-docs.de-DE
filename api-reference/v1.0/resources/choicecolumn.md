---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: c266550e8918603c3ee6104818c0aa721f1281d9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="85e57-102">ChoiceColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="85e57-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="85e57-103">Die **ChoiceColumn** einer [ColumnDefinition](columnDefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer Auswahlliste ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="85e57-103">The **choiceColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85e57-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="85e57-104">JSON representation</span></span>

<span data-ttu-id="85e57-105">Es folgt eine JSON-Darstellung einer **choiceColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="85e57-105">Here is a JSON representation of a **drive** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="85e57-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="85e57-106">Properties</span></span>

| <span data-ttu-id="85e57-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="85e57-107">Property name</span></span>      | <span data-ttu-id="85e57-108">Typ</span><span class="sxs-lookup"><span data-stu-id="85e57-108">Type</span></span>               | <span data-ttu-id="85e57-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85e57-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="85e57-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="85e57-110">**allowTextEntry**</span></span> | <span data-ttu-id="85e57-111">boolean</span><span class="sxs-lookup"><span data-stu-id="85e57-111">boolean</span></span>            | <span data-ttu-id="85e57-112">Ist der Wert true, sind benutzerdefinierte Werte, die sich nicht in der konfigurierten Auswahl befinden, zugelassen.</span><span class="sxs-lookup"><span data-stu-id="85e57-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="85e57-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="85e57-113">**CHOICES**</span></span>        | <span data-ttu-id="85e57-114">Collection(string)</span><span class="sxs-lookup"><span data-stu-id="85e57-114">Collection(String)</span></span> | <span data-ttu-id="85e57-115">Die Liste der Werte, die für diese Spalte zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="85e57-115">The list of values available for this column.</span></span>
| <span data-ttu-id="85e57-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="85e57-116">**displayAs**</span></span>      | <span data-ttu-id="85e57-117">string</span><span class="sxs-lookup"><span data-stu-id="85e57-117">string</span></span>             | <span data-ttu-id="85e57-118">Wie werden die Auswahlmöglichkeiten in der UX dargestellt?</span><span class="sxs-lookup"><span data-stu-id="85e57-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="85e57-119">Muss `checkBoxes`, `dropDownMenu` oder `radioButtons` sein.</span><span class="sxs-lookup"><span data-stu-id="85e57-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
