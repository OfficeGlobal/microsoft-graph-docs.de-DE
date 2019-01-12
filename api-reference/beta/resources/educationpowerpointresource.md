---
title: Ressourcentyp educationPowerPointResource
description: 'Eine Unterklasse der EducationResource. Hierbei handelt es sich um eine PowerPoint-Ressource. PowerPoint-Datei muss im Zusammenhang mit **FileResource** Verzeichnis hochgeladen werden die '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f92d74d8e3dfb7cebcecd607bbd4bd8e2f3b43da
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940666"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="2584a-105">Ressourcentyp educationPowerPointResource</span><span class="sxs-lookup"><span data-stu-id="2584a-105">educationPowerPointResource resource type</span></span>

> <span data-ttu-id="2584a-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2584a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2584a-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2584a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2584a-108">Eine Unterklasse der [EducationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="2584a-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="2584a-109">Hierbei handelt es sich um eine PowerPoint-Ressource.</span><span class="sxs-lookup"><span data-stu-id="2584a-109">This is a PowerPoint resource.</span></span> <span data-ttu-id="2584a-110">PowerPoint-Datei muss im Verzeichnis **FileResource** zugeordnet, die Zuordnung oder die Übermittlung hochgeladen werden.</span><span class="sxs-lookup"><span data-stu-id="2584a-110">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="2584a-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2584a-111">Properties</span></span>
| <span data-ttu-id="2584a-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2584a-112">Property</span></span>     | <span data-ttu-id="2584a-113">Typ</span><span class="sxs-lookup"><span data-stu-id="2584a-113">Type</span></span>   |<span data-ttu-id="2584a-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2584a-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2584a-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="2584a-115">fileUrl</span></span>|<span data-ttu-id="2584a-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2584a-116">String</span></span>|<span data-ttu-id="2584a-117">Speicherort der Datei auf dem Datenträger.</span><span class="sxs-lookup"><span data-stu-id="2584a-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2584a-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2584a-118">JSON representation</span></span>

<span data-ttu-id="2584a-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2584a-119">The following is a JSON representation of the resource.</span></span>

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
