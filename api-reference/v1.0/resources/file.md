---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Datei
localization_priority: Normal
ms.openlocfilehash: 7478ba064b5193ce7ddcd8685fc571a72d4b0057
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480407"
---
# <a name="file-resource-type"></a><span data-ttu-id="e7dc7-102">File-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e7dc7-102">File resource type</span></span>

<span data-ttu-id="e7dc7-103">Die **File**-Ressource gruppiert dateibezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="e7dc7-103">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="e7dc7-p101">Wenn ein [**DriveItem**](driveitem.md) ein **file**-Facet ungleich Null aufweist, stellt das Element eine Datei dar. Neben anderen Eigenschaften weisen Dateien eine **content**-Beziehung auf, die den Bytedatenstrom der Datei enthält.</span><span class="sxs-lookup"><span data-stu-id="e7dc7-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7dc7-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e7dc7-106">JSON representation</span></span>

<span data-ttu-id="e7dc7-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e7dc7-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a><span data-ttu-id="e7dc7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e7dc7-108">Properties</span></span>

| <span data-ttu-id="e7dc7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e7dc7-109">Property</span></span> | <span data-ttu-id="e7dc7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e7dc7-110">Type</span></span>                    | <span data-ttu-id="e7dc7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7dc7-111">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e7dc7-112">hashes</span><span class="sxs-lookup"><span data-stu-id="e7dc7-112">hashes</span></span>   | [<span data-ttu-id="e7dc7-113">Hashes</span><span class="sxs-lookup"><span data-stu-id="e7dc7-113">Hashes</span></span>](hashes.md) | <span data-ttu-id="e7dc7-p102">Hashes des binären Inhalts der Datei, wenn verfügbar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e7dc7-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="e7dc7-116">mimeType</span><span class="sxs-lookup"><span data-stu-id="e7dc7-116">mimeType</span></span> | <span data-ttu-id="e7dc7-117">string</span><span class="sxs-lookup"><span data-stu-id="e7dc7-117">string</span></span>                  | <span data-ttu-id="e7dc7-p103">Der MIME-Typ für die Datei. Dieser wird von der Logik auf dem Server bestimmt und stimmt möglicherweise nicht mit dem Wert überein, der bereitgestellt wurde, als die Datei hochgeladen wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e7dc7-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="e7dc7-121">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="e7dc7-121">Remarks</span></span> 

<span data-ttu-id="e7dc7-122">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e7dc7-122">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
