---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 21405fe3aa28e0eef1233cd6f27e63568fb4b00e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482217"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="8947c-102">ChoiceColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8947c-102">ChoiceColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8947c-103">Die **ChoiceColumn** einer [ColumnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte aus einer Auswahlliste ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="8947c-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8947c-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8947c-104">JSON representation</span></span>

<span data-ttu-id="8947c-105">Es folgt eine JSON-Darstellung einer **choiceColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="8947c-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="8947c-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8947c-106">Properties</span></span>

| <span data-ttu-id="8947c-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="8947c-107">Property name</span></span>      | <span data-ttu-id="8947c-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8947c-108">Type</span></span>               | <span data-ttu-id="8947c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8947c-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="8947c-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="8947c-110">**allowTextEntry**</span></span> | <span data-ttu-id="8947c-111">boolean</span><span class="sxs-lookup"><span data-stu-id="8947c-111">boolean</span></span>            | <span data-ttu-id="8947c-112">Ist der Wert true, sind benutzerdefinierte Werte, die sich nicht in der konfigurierten Auswahl befinden, zugelassen.</span><span class="sxs-lookup"><span data-stu-id="8947c-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="8947c-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="8947c-113">**choices**</span></span>        | <span data-ttu-id="8947c-114">Collection(string)</span><span class="sxs-lookup"><span data-stu-id="8947c-114">collection(string)</span></span> | <span data-ttu-id="8947c-115">Die Liste der Werte, die für diese Spalte zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="8947c-115">The list of values available for this column.</span></span>
| <span data-ttu-id="8947c-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="8947c-116">**displayAs**</span></span>      | <span data-ttu-id="8947c-117">string</span><span class="sxs-lookup"><span data-stu-id="8947c-117">string</span></span>             | <span data-ttu-id="8947c-118">Wie werden die Auswahlmöglichkeiten in der UX dargestellt?</span><span class="sxs-lookup"><span data-stu-id="8947c-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="8947c-119">Muss `checkBoxes`, `dropDownMenu` oder `radioButtons` sein.</span><span class="sxs-lookup"><span data-stu-id="8947c-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/choicecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
