---
title: Anwendung Ressourcentyp
description: Stellt die Excel-Anwendung dar, die die Arbeitsmappe verwaltet.
ms.openlocfilehash: 1772d69b55d03bf62d983a6dfb818dca651ebbd6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061371"
---
# <a name="application-resource-type"></a><span data-ttu-id="058fe-103">Anwendung Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="058fe-103">Application resource type</span></span>

> <span data-ttu-id="058fe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="058fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="058fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="058fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="058fe-106">Stellt die Excel-Anwendung dar, die die Arbeitsmappe verwaltet.</span><span class="sxs-lookup"><span data-stu-id="058fe-106">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="058fe-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="058fe-107">Methods</span></span>

| <span data-ttu-id="058fe-108">Methode</span><span class="sxs-lookup"><span data-stu-id="058fe-108">Method</span></span>           | <span data-ttu-id="058fe-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="058fe-109">Return Type</span></span>    |<span data-ttu-id="058fe-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="058fe-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="058fe-111">Abrufen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="058fe-111">Get Application</span></span>](../api/excelapplication-get.md) | [<span data-ttu-id="058fe-112">Application</span><span class="sxs-lookup"><span data-stu-id="058fe-112">Application</span></span>](application.md) |<span data-ttu-id="058fe-113">Lesen Sie Eigenschaften und Beziehungen des Application-Objekts.</span><span class="sxs-lookup"><span data-stu-id="058fe-113">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="058fe-114">Calculate</span><span class="sxs-lookup"><span data-stu-id="058fe-114">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="058fe-115">Keines</span><span class="sxs-lookup"><span data-stu-id="058fe-115">None</span></span>|<span data-ttu-id="058fe-116">Alle in Excel geöffnete Arbeitsmappen werden neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="058fe-116">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="058fe-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="058fe-117">Properties</span></span>
| <span data-ttu-id="058fe-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="058fe-118">Property</span></span>     | <span data-ttu-id="058fe-119">Typ</span><span class="sxs-lookup"><span data-stu-id="058fe-119">Type</span></span>   |<span data-ttu-id="058fe-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="058fe-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="058fe-121">calculationMode</span><span class="sxs-lookup"><span data-stu-id="058fe-121">calculationMode</span></span>|<span data-ttu-id="058fe-122">string</span><span class="sxs-lookup"><span data-stu-id="058fe-122">string</span></span>|<span data-ttu-id="058fe-123">Gibt den Berechnungsmodus in der Arbeitsmappe verwendet.</span><span class="sxs-lookup"><span data-stu-id="058fe-123">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="058fe-124">Mögliche Werte sind: `Automatic`, `AutomaticExceptTables` und `Manual`.</span><span class="sxs-lookup"><span data-stu-id="058fe-124">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="058fe-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="058fe-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="058fe-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="058fe-126">Relationships</span></span>
<span data-ttu-id="058fe-127">Keine</span><span class="sxs-lookup"><span data-stu-id="058fe-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="058fe-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="058fe-128">JSON representation</span></span>

<span data-ttu-id="058fe-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="058fe-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->