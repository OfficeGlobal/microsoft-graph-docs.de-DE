---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
ms.openlocfilehash: 9de6923146b915207fc771721d7aeb6767e9f99e
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="hashes-resource-type"></a><span data-ttu-id="00aac-101">Hash-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="00aac-101">Hashes resource type</span></span>

<span data-ttu-id="00aac-102">Die **Hashes**-Ressourcengruppen machen Hashes in einer einzelnen Struktur für ein Element verfügbar.</span><span class="sxs-lookup"><span data-stu-id="00aac-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="00aac-103">**Hinweis:** Nicht alle Dienste geben einen Wert für alle aufgeführten Hash-Eigenschaften an.</span><span class="sxs-lookup"><span data-stu-id="00aac-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="00aac-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="00aac-104">JSON representation</span></span>

<span data-ttu-id="00aac-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="00aac-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="00aac-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="00aac-106">Properties</span></span>

| <span data-ttu-id="00aac-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00aac-107">Property</span></span>         | <span data-ttu-id="00aac-108">Typ</span><span class="sxs-lookup"><span data-stu-id="00aac-108">Type</span></span>   | <span data-ttu-id="00aac-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00aac-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="00aac-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="00aac-110">**sha1Hash**</span></span>     | <span data-ttu-id="00aac-111">String</span><span class="sxs-lookup"><span data-stu-id="00aac-111">String</span></span> | <span data-ttu-id="00aac-p101">SHA1-Hash für den Inhalt der Datei (sofern zutreffend). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="00aac-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="00aac-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="00aac-114">**crc32Hash**</span></span>    | <span data-ttu-id="00aac-115">String</span><span class="sxs-lookup"><span data-stu-id="00aac-115">String</span></span> | <span data-ttu-id="00aac-p102">Der Wert der CRC32 der Datei (sofern zutreffend). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="00aac-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="00aac-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="00aac-118">**quickXorHash**</span></span> | <span data-ttu-id="00aac-119">String</span><span class="sxs-lookup"><span data-stu-id="00aac-119">String</span></span> | <span data-ttu-id="00aac-p103">Ein proprietärer Hash der Datei, die verwendet werden kann, um festzustellen, ob sich der Inhalt der Datei (sofern zutreffend) geändert hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="00aac-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="00aac-p104">**Hinweis:** In einigen Fällen stehen möglicherweise keine Hash-Werte zur Verfügung. Wenn dies der Fall ist, werden die Hash-Werte für ein Element nach dem Download des Elements aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="00aac-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="00aac-124">Hinweise</span><span class="sxs-lookup"><span data-stu-id="00aac-124">Remarks</span></span>

<span data-ttu-id="00aac-125">In OneDrive for Business und SharePoint Server 2016 sind **sha1Hash** und **crc32Hash** nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="00aac-125">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="00aac-126">In OneDrive Personal ist **quickXorHash** nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="00aac-126">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="00aac-127">Wie Sie **quickXorHash** für eine Datei berechnen, illustriert [dieser Codeausschnitt zu „quickXorHash“](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="00aac-127">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="00aac-128">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="00aac-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
