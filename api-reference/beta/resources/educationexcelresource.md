---
title: Ressourcentyp educationExcelResource
description: 'Eine Unterklasse der EducationResource. Dieser Ressourcentyp stellt ein Excel-Dokument dar.  '
ms.openlocfilehash: cdd86cf1048863ac3def2ae6be13c3f39b37e642
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065154"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="fe70d-104">Ressourcentyp educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="fe70d-104">educationExcelResource resource type</span></span>

> <span data-ttu-id="fe70d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fe70d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe70d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe70d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe70d-107">Eine Unterklasse der [EducationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="fe70d-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="fe70d-108">Dieser Ressourcentyp stellt ein Excel-Dokument dar.</span><span class="sxs-lookup"><span data-stu-id="fe70d-108">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="fe70d-109">**Hinweis:** Die Excel-Datei muss im Ordner "Resource" die Zuordnung oder Übermittlung-Objekt zu dem diese Ressource gehört zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="fe70d-109">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="fe70d-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fe70d-110">Properties</span></span>
| <span data-ttu-id="fe70d-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fe70d-111">Property</span></span>     | <span data-ttu-id="fe70d-112">Typ</span><span class="sxs-lookup"><span data-stu-id="fe70d-112">Type</span></span>   |<span data-ttu-id="fe70d-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe70d-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe70d-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="fe70d-114">fileUrl</span></span>|<span data-ttu-id="fe70d-115">String</span><span class="sxs-lookup"><span data-stu-id="fe70d-115">String</span></span>|<span data-ttu-id="fe70d-116">Zeiger auf das Excel-File-Objekt.</span><span class="sxs-lookup"><span data-stu-id="fe70d-116">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe70d-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fe70d-117">JSON representation</span></span>

<span data-ttu-id="fe70d-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fe70d-118">The following is a JSON representation of the resource.</span></span>

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