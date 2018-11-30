---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Hashes
ms.openlocfilehash: 2387af83450f667aa4732cc46d7d3cf2111579f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058439"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="4e73b-102">Hash-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4e73b-102">Hashes resource type</span></span>

> <span data-ttu-id="4e73b-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4e73b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e73b-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e73b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e73b-105">Die **Hashes**-Ressourcengruppen machen Hashes in einer einzelnen Struktur für ein Element verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4e73b-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="4e73b-106">**Hinweis:** Nicht alle Dienste geben einen Wert für alle aufgeführten Hash-Eigenschaften an.</span><span class="sxs-lookup"><span data-stu-id="4e73b-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e73b-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4e73b-107">JSON representation</span></span>

<span data-ttu-id="4e73b-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e73b-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4e73b-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4e73b-109">Properties</span></span>

| <span data-ttu-id="4e73b-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e73b-110">Property</span></span>         | <span data-ttu-id="4e73b-111">Typ</span><span class="sxs-lookup"><span data-stu-id="4e73b-111">Type</span></span>   | <span data-ttu-id="4e73b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e73b-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="4e73b-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="4e73b-113">**sha1Hash**</span></span>     | <span data-ttu-id="4e73b-114">String</span><span class="sxs-lookup"><span data-stu-id="4e73b-114">String</span></span> | <span data-ttu-id="4e73b-p102">SHA1-Hash für den Inhalt der Datei (sofern zutreffend). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e73b-p102">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="4e73b-117">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="4e73b-117">**crc32Hash**</span></span>    | <span data-ttu-id="4e73b-118">String</span><span class="sxs-lookup"><span data-stu-id="4e73b-118">String</span></span> | <span data-ttu-id="4e73b-p103">Der Wert der CRC32 der Datei (sofern zutreffend). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e73b-p103">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="4e73b-121">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="4e73b-121">**quickXorHash**</span></span> | <span data-ttu-id="4e73b-122">String</span><span class="sxs-lookup"><span data-stu-id="4e73b-122">String</span></span> | <span data-ttu-id="4e73b-p104">Ein proprietärer Hash der Datei, die verwendet werden kann, um festzustellen, ob sich der Inhalt der Datei (sofern zutreffend) geändert hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e73b-p104">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="4e73b-p105">**Hinweis:** In einigen Fällen stehen möglicherweise keine Hash-Werte zur Verfügung. Wenn dies der Fall ist, werden die Hash-Werte für ein Element nach dem Download des Elements aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4e73b-p105">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="4e73b-127">Hinweise</span><span class="sxs-lookup"><span data-stu-id="4e73b-127">Remarks</span></span>

<span data-ttu-id="4e73b-128">In OneDrive for Business und SharePoint Server 2016 sind **sha1Hash** und **crc32Hash** nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4e73b-128">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="4e73b-129">In OneDrive Personal ist **quickXorHash** nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4e73b-129">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="4e73b-130">Wie Sie **quickXorHash** für eine Datei berechnen, bezieht sich dieser auf den [quickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm)-Codeausschnitt.</span><span class="sxs-lookup"><span data-stu-id="4e73b-130">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>

<span data-ttu-id="4e73b-131">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4e73b-131">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
