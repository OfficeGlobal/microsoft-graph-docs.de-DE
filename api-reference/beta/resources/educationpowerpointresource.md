---
title: Ressourcentyp educationPowerPointResource
description: 'Eine Unterklasse der EducationResource. Hierbei handelt es sich um eine PowerPoint-Ressource. PowerPoint-Datei muss im Zusammenhang mit **FileResource** Verzeichnis hochgeladen werden die '
localization_priority: Normal
ms.openlocfilehash: 763a529e97b12c93d8f10aa6855c20818c02da67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845458"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="59f46-105">Ressourcentyp educationPowerPointResource</span><span class="sxs-lookup"><span data-stu-id="59f46-105">educationPowerPointResource resource type</span></span>

> <span data-ttu-id="59f46-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="59f46-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59f46-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="59f46-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59f46-108">Eine Unterklasse der [EducationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="59f46-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="59f46-109">Hierbei handelt es sich um eine PowerPoint-Ressource.</span><span class="sxs-lookup"><span data-stu-id="59f46-109">This is a PowerPoint resource.</span></span> <span data-ttu-id="59f46-110">PowerPoint-Datei muss im Verzeichnis **FileResource** zugeordnet, die Zuordnung oder die Übermittlung hochgeladen werden.</span><span class="sxs-lookup"><span data-stu-id="59f46-110">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="59f46-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="59f46-111">Properties</span></span>
| <span data-ttu-id="59f46-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="59f46-112">Property</span></span>     | <span data-ttu-id="59f46-113">Typ</span><span class="sxs-lookup"><span data-stu-id="59f46-113">Type</span></span>   |<span data-ttu-id="59f46-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59f46-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59f46-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="59f46-115">fileUrl</span></span>|<span data-ttu-id="59f46-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="59f46-116">String</span></span>|<span data-ttu-id="59f46-117">Speicherort der Datei auf dem Datenträger.</span><span class="sxs-lookup"><span data-stu-id="59f46-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59f46-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="59f46-118">JSON representation</span></span>

<span data-ttu-id="59f46-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="59f46-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
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
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
