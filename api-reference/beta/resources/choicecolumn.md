---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 2e0798f558ace72f59a6acccc0cc8ce3eb6e2291
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842546"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="c7cc7-102">ChoiceColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c7cc7-102">ChoiceColumn resource type</span></span>

> <span data-ttu-id="c7cc7-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c7cc7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7cc7-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7cc7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7cc7-105">Die **ChoiceColumn** einer [ColumnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer Auswahlliste ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="c7cc7-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7cc7-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7cc7-106">JSON representation</span></span>

<span data-ttu-id="c7cc7-107">Es folgt eine JSON-Darstellung einer **choiceColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7cc7-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="c7cc7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7cc7-108">Properties</span></span>

| <span data-ttu-id="c7cc7-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="c7cc7-109">Property name</span></span>      | <span data-ttu-id="c7cc7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c7cc7-110">Type</span></span>               | <span data-ttu-id="c7cc7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7cc7-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="c7cc7-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="c7cc7-112">**allowTextEntry**</span></span> | <span data-ttu-id="c7cc7-113">boolean</span><span class="sxs-lookup"><span data-stu-id="c7cc7-113">boolean</span></span>            | <span data-ttu-id="c7cc7-114">Ist der Wert true, sind benutzerdefinierte Werte, die sich nicht in der konfigurierten Auswahl befinden, zugelassen.</span><span class="sxs-lookup"><span data-stu-id="c7cc7-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="c7cc7-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="c7cc7-115">**choices**</span></span>        | <span data-ttu-id="c7cc7-116">Collection(string)</span><span class="sxs-lookup"><span data-stu-id="c7cc7-116">collection(string)</span></span> | <span data-ttu-id="c7cc7-117">Die Liste der Werte, die für diese Spalte zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="c7cc7-117">The list of values available for this column.</span></span>
| <span data-ttu-id="c7cc7-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="c7cc7-118">**displayAs**</span></span>      | <span data-ttu-id="c7cc7-119">string</span><span class="sxs-lookup"><span data-stu-id="c7cc7-119">string</span></span>             | <span data-ttu-id="c7cc7-120">Wie werden die Auswahlmöglichkeiten in der UX dargestellt?</span><span class="sxs-lookup"><span data-stu-id="c7cc7-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="c7cc7-121">Muss `checkBoxes`, `dropDownMenu` oder `radioButtons` sein.</span><span class="sxs-lookup"><span data-stu-id="c7cc7-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
