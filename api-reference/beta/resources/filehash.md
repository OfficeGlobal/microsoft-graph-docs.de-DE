---
title: Ressourcentyp fileHash
description: Enthält Statusinformationen zu Dateihashes (cryptographic und der Speicherort).
ms.openlocfilehash: 8f283046efc9b4af181cb33fb4e9ca63e4892b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062396"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="35d7a-103">Ressourcentyp fileHash</span><span class="sxs-lookup"><span data-stu-id="35d7a-103">fileHash resource type</span></span>

<span data-ttu-id="35d7a-104">Enthält Statusinformationen zu Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="35d7a-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="35d7a-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="35d7a-105">Properties</span></span>

| <span data-ttu-id="35d7a-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="35d7a-106">Property</span></span>     | <span data-ttu-id="35d7a-107">Typ</span><span class="sxs-lookup"><span data-stu-id="35d7a-107">Type</span></span>        | <span data-ttu-id="35d7a-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35d7a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="35d7a-109">hashType</span><span class="sxs-lookup"><span data-stu-id="35d7a-109">hashType</span></span>|<span data-ttu-id="35d7a-110">[FileHashType](filehashtypeenumtype.md) -Enumeration</span><span class="sxs-lookup"><span data-stu-id="35d7a-110">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="35d7a-111">Hash-Dateityp.</span><span class="sxs-lookup"><span data-stu-id="35d7a-111">File hash type.</span></span> <span data-ttu-id="35d7a-112">Mögliche Werte: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="35d7a-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="35d7a-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="35d7a-113">hashValue</span></span>|<span data-ttu-id="35d7a-114">String</span><span class="sxs-lookup"><span data-stu-id="35d7a-114">String</span></span>|<span data-ttu-id="35d7a-115">Der Wert des Dateihash.</span><span class="sxs-lookup"><span data-stu-id="35d7a-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35d7a-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="35d7a-116">JSON representation</span></span>

<span data-ttu-id="35d7a-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="35d7a-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->