---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
ms.openlocfilehash: 551b09cee9fa662d357ee763b67ce78bea03425f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514845"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="ed4f2-102">Hash-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ed4f2-102">Hashes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed4f2-103">Die **Hashes**-Ressourcengruppen machen Hashes in einer einzelnen Struktur für ein Element verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ed4f2-103">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="ed4f2-104">**Hinweis:** Nicht alle Dienste geben einen Wert für alle aufgeführten Hash-Eigenschaften an.</span><span class="sxs-lookup"><span data-stu-id="ed4f2-104">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed4f2-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ed4f2-105">JSON representation</span></span>

<span data-ttu-id="ed4f2-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ed4f2-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a><span data-ttu-id="ed4f2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ed4f2-107">Properties</span></span>

| <span data-ttu-id="ed4f2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed4f2-108">Property</span></span>         | <span data-ttu-id="ed4f2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ed4f2-109">Type</span></span>   | <span data-ttu-id="ed4f2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed4f2-110">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="ed4f2-111">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="ed4f2-111">**sha1Hash**</span></span>     | <span data-ttu-id="ed4f2-112">String</span><span class="sxs-lookup"><span data-stu-id="ed4f2-112">String</span></span> | <span data-ttu-id="ed4f2-p101">SHA1-Hash für den Inhalt der Datei (sofern zutreffend). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed4f2-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="ed4f2-115">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="ed4f2-115">**crc32Hash**</span></span>    | <span data-ttu-id="ed4f2-116">String</span><span class="sxs-lookup"><span data-stu-id="ed4f2-116">String</span></span> | <span data-ttu-id="ed4f2-p102">Der Wert der CRC32 der Datei (sofern zutreffend). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed4f2-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="ed4f2-119">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="ed4f2-119">**quickXorHash**</span></span> | <span data-ttu-id="ed4f2-120">String</span><span class="sxs-lookup"><span data-stu-id="ed4f2-120">String</span></span> | <span data-ttu-id="ed4f2-p103">Ein proprietärer Hash der Datei, die verwendet werden kann, um festzustellen, ob sich der Inhalt der Datei (sofern zutreffend) geändert hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed4f2-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="ed4f2-p104">**Hinweis:** In einigen Fällen stehen möglicherweise keine Hash-Werte zur Verfügung. Wenn dies der Fall ist, werden die Hash-Werte für ein Element nach dem Download des Elements aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="ed4f2-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="ed4f2-125">Hinweise</span><span class="sxs-lookup"><span data-stu-id="ed4f2-125">Remarks</span></span>

<span data-ttu-id="ed4f2-126">In OneDrive for Business und SharePoint Server 2016 sind **sha1Hash** und **crc32Hash** nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ed4f2-126">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="ed4f2-127">In OneDrive Personal ist **quickXorHash** nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ed4f2-127">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="ed4f2-128">Wie Sie **quickXorHash** für eine Datei berechnen, bezieht sich dieser auf den [quickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm)-Codeausschnitt.</span><span class="sxs-lookup"><span data-stu-id="ed4f2-128">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>

<span data-ttu-id="ed4f2-129">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ed4f2-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": [
    "Error: /api-reference/beta/resources/hashes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
