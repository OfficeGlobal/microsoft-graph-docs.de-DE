---
title: Ressourcentyp fileSecurityState
description: Enthält Informationen zur Datei (nicht verarbeiten) im Zusammenhang mit der Benachrichtigung.
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894096"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="0c5ea-103">Ressourcentyp fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="0c5ea-103">fileSecurityState resource type</span></span>

<span data-ttu-id="0c5ea-104">Enthält Informationen zur Datei (nicht verarbeiten) im Zusammenhang mit der Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="0c5ea-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="0c5ea-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0c5ea-105">Properties</span></span>

| <span data-ttu-id="0c5ea-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0c5ea-106">Property</span></span>   | <span data-ttu-id="0c5ea-107">Typ</span><span class="sxs-lookup"><span data-stu-id="0c5ea-107">Type</span></span>|<span data-ttu-id="0c5ea-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c5ea-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c5ea-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="0c5ea-109">fileHash</span></span>|[<span data-ttu-id="0c5ea-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="0c5ea-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="0c5ea-111">Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="0c5ea-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="0c5ea-112">name</span><span class="sxs-lookup"><span data-stu-id="0c5ea-112">name</span></span>|<span data-ttu-id="0c5ea-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c5ea-113">String</span></span>|<span data-ttu-id="0c5ea-114">Der Dateiname (ohne Pfad).</span><span class="sxs-lookup"><span data-stu-id="0c5ea-114">File name (without path).</span></span>|
|<span data-ttu-id="0c5ea-115">Pfad</span><span class="sxs-lookup"><span data-stu-id="0c5ea-115">path</span></span>|<span data-ttu-id="0c5ea-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c5ea-116">String</span></span>|<span data-ttu-id="0c5ea-117">Vollständiger Dateipfad der die Datei/ImageFile.</span><span class="sxs-lookup"><span data-stu-id="0c5ea-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="0c5ea-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="0c5ea-118">riskScore</span></span>|<span data-ttu-id="0c5ea-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c5ea-119">String</span></span>|<span data-ttu-id="0c5ea-120">Anbieter generiert/berechnet riskieren Bewertung der alert-Datei.</span><span class="sxs-lookup"><span data-stu-id="0c5ea-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="0c5ea-121">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="0c5ea-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c5ea-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0c5ea-122">JSON representation</span></span>

<span data-ttu-id="0c5ea-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0c5ea-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
