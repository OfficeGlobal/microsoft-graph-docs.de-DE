---
title: Ressourcentyp educationExcelResource
description: 'Eine Unterklasse der EducationResource. Dieser Ressourcentyp stellt ein Excel-Dokument dar.  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 7f772f7911667c76e64c31a856f3a9f8b6f3e6ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858100"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="4a961-104">Ressourcentyp educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="4a961-104">educationExcelResource resource type</span></span>

> <span data-ttu-id="4a961-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4a961-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a961-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4a961-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a961-107">Eine Unterklasse der [EducationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="4a961-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="4a961-108">Dieser Ressourcentyp stellt ein Excel-Dokument dar.</span><span class="sxs-lookup"><span data-stu-id="4a961-108">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="4a961-109">**Hinweis:** Die Excel-Datei muss im Ordner "Resource" die Zuordnung oder Übermittlung-Objekt zu dem diese Ressource gehört zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="4a961-109">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="4a961-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4a961-110">Properties</span></span>
| <span data-ttu-id="4a961-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4a961-111">Property</span></span>     | <span data-ttu-id="4a961-112">Typ</span><span class="sxs-lookup"><span data-stu-id="4a961-112">Type</span></span>   |<span data-ttu-id="4a961-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a961-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a961-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="4a961-114">fileUrl</span></span>|<span data-ttu-id="4a961-115">String</span><span class="sxs-lookup"><span data-stu-id="4a961-115">String</span></span>|<span data-ttu-id="4a961-116">Zeiger auf das Excel-File-Objekt.</span><span class="sxs-lookup"><span data-stu-id="4a961-116">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a961-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4a961-117">JSON representation</span></span>

<span data-ttu-id="4a961-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4a961-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
