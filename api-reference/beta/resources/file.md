---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Datei
ms.openlocfilehash: bd0cd6ea5f5ee2225392aa61c2dda9b30e2ffbca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064196"
---
# <a name="file-resource-type"></a><span data-ttu-id="93a7d-102">File-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="93a7d-102">File resource type</span></span>

> <span data-ttu-id="93a7d-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="93a7d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93a7d-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93a7d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93a7d-105">Die **File**-Ressource gruppiert dateibezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="93a7d-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="93a7d-p102">Wenn ein [**DriveItem**](driveitem.md) ein **file**-Facet ungleich Null aufweist, stellt das Element eine Datei dar. Neben anderen Eigenschaften weisen Dateien eine **content**-Beziehung auf, die den Bytedatenstrom der Datei enthält.</span><span class="sxs-lookup"><span data-stu-id="93a7d-p102">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93a7d-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="93a7d-108">JSON representation</span></span>

<span data-ttu-id="93a7d-109">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="93a7d-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="93a7d-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="93a7d-110">Properties</span></span>

| <span data-ttu-id="93a7d-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93a7d-111">Property</span></span> | <span data-ttu-id="93a7d-112">Typ</span><span class="sxs-lookup"><span data-stu-id="93a7d-112">Type</span></span>                    | <span data-ttu-id="93a7d-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93a7d-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="93a7d-114">hashes</span><span class="sxs-lookup"><span data-stu-id="93a7d-114">hashes</span></span>   | [<span data-ttu-id="93a7d-115">HashesType</span><span class="sxs-lookup"><span data-stu-id="93a7d-115">HashesType</span></span>](hashes.md) | <span data-ttu-id="93a7d-p103">Hashes des binären Inhalts der Datei, wenn verfügbar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="93a7d-p103">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="93a7d-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="93a7d-118">mimeType</span></span> | <span data-ttu-id="93a7d-119">string</span><span class="sxs-lookup"><span data-stu-id="93a7d-119">string</span></span>                  | <span data-ttu-id="93a7d-p104">Der MIME-Typ für die Datei. Dieser wird von der Logik auf dem Server bestimmt und stimmt möglicherweise nicht mit dem Wert überein, der bereitgestellt wurde, als die Datei hochgeladen wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="93a7d-p104">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="93a7d-123">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="93a7d-123">Remarks</span></span> 

<span data-ttu-id="93a7d-124">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="93a7d-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
