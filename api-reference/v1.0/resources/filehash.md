---
title: Ressourcentyp fileHash
description: Enthält Statusinformationen zu Dateihashes (cryptographic und der Speicherort).
localization_priority: Normal
ms.openlocfilehash: 9d72812d1ad43999ea3ed5b28251d629b9380d47
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876769"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="86ca5-103">Ressourcentyp fileHash</span><span class="sxs-lookup"><span data-stu-id="86ca5-103">fileHash resource type</span></span>

<span data-ttu-id="86ca5-104">Enthält Statusinformationen zu Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="86ca5-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="86ca5-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="86ca5-105">Properties</span></span>

| <span data-ttu-id="86ca5-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86ca5-106">Property</span></span>     | <span data-ttu-id="86ca5-107">Typ</span><span class="sxs-lookup"><span data-stu-id="86ca5-107">Type</span></span>        | <span data-ttu-id="86ca5-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86ca5-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86ca5-109">hashType</span><span class="sxs-lookup"><span data-stu-id="86ca5-109">hashType</span></span>|<span data-ttu-id="86ca5-110">fileHashType</span><span class="sxs-lookup"><span data-stu-id="86ca5-110">fileHashType</span></span>|<span data-ttu-id="86ca5-111">Hash-Dateityp.</span><span class="sxs-lookup"><span data-stu-id="86ca5-111">File hash type.</span></span> <span data-ttu-id="86ca5-112">Mögliche Werte: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="86ca5-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="86ca5-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="86ca5-113">hashValue</span></span>|<span data-ttu-id="86ca5-114">String</span><span class="sxs-lookup"><span data-stu-id="86ca5-114">String</span></span>|<span data-ttu-id="86ca5-115">Der Wert des Dateihash.</span><span class="sxs-lookup"><span data-stu-id="86ca5-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86ca5-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="86ca5-116">JSON representation</span></span>

<span data-ttu-id="86ca5-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="86ca5-117">The following is a JSON representation of the resource.</span></span>

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
