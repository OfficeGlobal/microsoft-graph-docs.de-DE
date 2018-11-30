---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: 659ece2eab255fe7b55a258b0980eda4e7bde5b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058158"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="7f28f-102">ChoiceColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7f28f-102">ChoiceColumn resource type</span></span>

> <span data-ttu-id="7f28f-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7f28f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f28f-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7f28f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f28f-105">Die **ChoiceColumn** einer [ColumnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer Auswahlliste ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="7f28f-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f28f-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7f28f-106">JSON representation</span></span>

<span data-ttu-id="7f28f-107">Es folgt eine JSON-Darstellung einer **choiceColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="7f28f-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="7f28f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7f28f-108">Properties</span></span>

| <span data-ttu-id="7f28f-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="7f28f-109">Property name</span></span>      | <span data-ttu-id="7f28f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7f28f-110">Type</span></span>               | <span data-ttu-id="7f28f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f28f-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="7f28f-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="7f28f-112">**allowTextEntry**</span></span> | <span data-ttu-id="7f28f-113">boolean</span><span class="sxs-lookup"><span data-stu-id="7f28f-113">boolean</span></span>            | <span data-ttu-id="7f28f-114">Ist der Wert true, sind benutzerdefinierte Werte, die sich nicht in der konfigurierten Auswahl befinden, zugelassen.</span><span class="sxs-lookup"><span data-stu-id="7f28f-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="7f28f-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="7f28f-115">**choices**</span></span>        | <span data-ttu-id="7f28f-116">Collection(string)</span><span class="sxs-lookup"><span data-stu-id="7f28f-116">collection(string)</span></span> | <span data-ttu-id="7f28f-117">Die Liste der Werte, die für diese Spalte zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="7f28f-117">The list of values available for this column.</span></span>
| <span data-ttu-id="7f28f-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="7f28f-118">**displayAs**</span></span>      | <span data-ttu-id="7f28f-119">string</span><span class="sxs-lookup"><span data-stu-id="7f28f-119">string</span></span>             | <span data-ttu-id="7f28f-120">Wie werden die Auswahlmöglichkeiten in der UX dargestellt?</span><span class="sxs-lookup"><span data-stu-id="7f28f-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="7f28f-121">Muss `checkBoxes`, `dropDownMenu` oder `radioButtons` sein.</span><span class="sxs-lookup"><span data-stu-id="7f28f-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
