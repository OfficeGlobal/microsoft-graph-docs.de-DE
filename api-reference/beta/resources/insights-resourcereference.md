---
title: Ressourcentyp resourceReference
description: Komplexer Typ mit Eigenschaften des Insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 23a05a362ea57c84dceecbd9523c2620edc21fbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966286"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="5b779-103">Ressourcentyp resourceReference</span><span class="sxs-lookup"><span data-stu-id="5b779-103">resourceReference resource type</span></span>

> <span data-ttu-id="5b779-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5b779-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b779-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b779-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b779-106">Komplexer Typ mit Eigenschaften des [Insights](insights.md).</span><span class="sxs-lookup"><span data-stu-id="5b779-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b779-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5b779-107">JSON representation</span></span>

<span data-ttu-id="5b779-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5b779-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="5b779-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5b779-109">Properties</span></span>

| <span data-ttu-id="5b779-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5b779-110">Property</span></span>      | <span data-ttu-id="5b779-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5b779-111">Type</span></span>      | <span data-ttu-id="5b779-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b779-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="5b779-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="5b779-113">webUrl</span></span>        | <span data-ttu-id="5b779-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5b779-114">String</span></span>    | <span data-ttu-id="5b779-115">Eine URL, die auf das verwiesene Element führende.</span><span class="sxs-lookup"><span data-stu-id="5b779-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="5b779-116">id</span><span class="sxs-lookup"><span data-stu-id="5b779-116">id</span></span>            | <span data-ttu-id="5b779-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5b779-117">String</span></span>    | <span data-ttu-id="5b779-118">Eindeutiger Bezeichner des Elements.</span><span class="sxs-lookup"><span data-stu-id="5b779-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="5b779-119">type</span><span class="sxs-lookup"><span data-stu-id="5b779-119">type</span></span>          | <span data-ttu-id="5b779-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5b779-120">String</span></span>    | <span data-ttu-id="5b779-121">Ein String-Wert, der verwendet werden kann, um das Element, wie beispielsweise "microsoft.graph.driveItem" klassifizieren</span><span class="sxs-lookup"><span data-stu-id="5b779-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
