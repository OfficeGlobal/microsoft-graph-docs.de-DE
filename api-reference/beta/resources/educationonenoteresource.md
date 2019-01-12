---
title: Ressourcentyp educationOneNoteResource
description: 'Eine Unterklasse der EducationResource. Dies ist den Speicherort der OneNote-Seite.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b10bef551cdc2dd29a8a20c69d2c4657ee66af4e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927919"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="01f0d-104">Ressourcentyp educationOneNoteResource</span><span class="sxs-lookup"><span data-stu-id="01f0d-104">educationOneNoteResource resource type</span></span>

> <span data-ttu-id="01f0d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="01f0d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01f0d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="01f0d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01f0d-107">Eine Unterklasse der [EducationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="01f0d-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="01f0d-108">Dies ist den Speicherort der OneNote-Seite.</span><span class="sxs-lookup"><span data-stu-id="01f0d-108">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="01f0d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="01f0d-109">Properties</span></span>
| <span data-ttu-id="01f0d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="01f0d-110">Property</span></span>     | <span data-ttu-id="01f0d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="01f0d-111">Type</span></span>   |<span data-ttu-id="01f0d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01f0d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01f0d-113">pageUrl</span><span class="sxs-lookup"><span data-stu-id="01f0d-113">pageUrl</span></span>|<span data-ttu-id="01f0d-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01f0d-114">String</span></span>|<span data-ttu-id="01f0d-115">Die Microsoft Graph-URL zu der Seite in OneNote.</span><span class="sxs-lookup"><span data-stu-id="01f0d-115">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="01f0d-116">sectionName</span><span class="sxs-lookup"><span data-stu-id="01f0d-116">sectionName</span></span>|<span data-ttu-id="01f0d-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01f0d-117">String</span></span>|<span data-ttu-id="01f0d-118">Im Abschnittsname, die Verteilung in kopiert werden sollte oder in kopiert wurden.</span><span class="sxs-lookup"><span data-stu-id="01f0d-118">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01f0d-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="01f0d-119">JSON representation</span></span>

<span data-ttu-id="01f0d-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="01f0d-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
