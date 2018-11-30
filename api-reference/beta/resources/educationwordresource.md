---
title: Ressourcentyp educationWordResource
description: 'Eine Unterklasse der EducationResource. Hierbei handelt es sich um eine Word-Dokument-Ressource. Die Word-Datei muss im Zusammenhang mit **FileResource** Verzeichnis hochgeladen werden die '
ms.openlocfilehash: 28df3278a0d97f440014c342d592d2701b348d94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063534"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="a0117-105">Ressourcentyp educationWordResource</span><span class="sxs-lookup"><span data-stu-id="a0117-105">educationWordResource resource type</span></span>

> <span data-ttu-id="a0117-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a0117-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0117-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a0117-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0117-108">Eine Unterklasse der [EducationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="a0117-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="a0117-109">Hierbei handelt es sich um eine Word-Dokument-Ressource.</span><span class="sxs-lookup"><span data-stu-id="a0117-109">This is a Word document resource.</span></span> <span data-ttu-id="a0117-110">Die Word-Datei muss im Verzeichnis **FileResource** zugeordnet, die Zuordnung oder die Übermittlung hochgeladen werden.</span><span class="sxs-lookup"><span data-stu-id="a0117-110">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="a0117-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a0117-111">Properties</span></span>
| <span data-ttu-id="a0117-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a0117-112">Property</span></span>     | <span data-ttu-id="a0117-113">Typ</span><span class="sxs-lookup"><span data-stu-id="a0117-113">Type</span></span>   |<span data-ttu-id="a0117-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0117-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0117-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="a0117-115">fileUrl</span></span>|<span data-ttu-id="a0117-116">String</span><span class="sxs-lookup"><span data-stu-id="a0117-116">String</span></span>|<span data-ttu-id="a0117-117">Speicherort der Datei auf dem Datenträger.</span><span class="sxs-lookup"><span data-stu-id="a0117-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0117-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a0117-118">JSON representation</span></span>

<span data-ttu-id="a0117-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a0117-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
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
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->