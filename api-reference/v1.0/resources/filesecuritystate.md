---
title: Ressourcentyp fileSecurityState
description: Enthält Informationen zur Datei (nicht verarbeiten) im Zusammenhang mit der Benachrichtigung.
ms.openlocfilehash: d1358d7fe0d5565845201781e32b3da14a89f412
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019795"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="b17c1-103">Ressourcentyp fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="b17c1-103">fileSecurityState resource type</span></span>

<span data-ttu-id="b17c1-104">Enthält Informationen zur Datei (nicht verarbeiten) im Zusammenhang mit der Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="b17c1-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="b17c1-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b17c1-105">Properties</span></span>

| <span data-ttu-id="b17c1-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b17c1-106">Property</span></span>   | <span data-ttu-id="b17c1-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b17c1-107">Type</span></span>|<span data-ttu-id="b17c1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b17c1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b17c1-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="b17c1-109">fileHash</span></span>|[<span data-ttu-id="b17c1-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="b17c1-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="b17c1-111">Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="b17c1-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="b17c1-112">name</span><span class="sxs-lookup"><span data-stu-id="b17c1-112">name</span></span>|<span data-ttu-id="b17c1-113">String</span><span class="sxs-lookup"><span data-stu-id="b17c1-113">String</span></span>|<span data-ttu-id="b17c1-114">Der Dateiname (ohne Pfad).</span><span class="sxs-lookup"><span data-stu-id="b17c1-114">File name (without path).</span></span>|
|<span data-ttu-id="b17c1-115">Pfad</span><span class="sxs-lookup"><span data-stu-id="b17c1-115">path</span></span>|<span data-ttu-id="b17c1-116">String</span><span class="sxs-lookup"><span data-stu-id="b17c1-116">String</span></span>|<span data-ttu-id="b17c1-117">Vollständiger Dateipfad der die Datei/ImageFile.</span><span class="sxs-lookup"><span data-stu-id="b17c1-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="b17c1-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="b17c1-118">riskScore</span></span>|<span data-ttu-id="b17c1-119">String</span><span class="sxs-lookup"><span data-stu-id="b17c1-119">String</span></span>|<span data-ttu-id="b17c1-120">Anbieter generiert/berechnet riskieren Bewertung der alert-Datei.</span><span class="sxs-lookup"><span data-stu-id="b17c1-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="b17c1-121">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="b17c1-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b17c1-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b17c1-122">JSON representation</span></span>

<span data-ttu-id="b17c1-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b17c1-123">The following is a JSON representation of the resource.</span></span>

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