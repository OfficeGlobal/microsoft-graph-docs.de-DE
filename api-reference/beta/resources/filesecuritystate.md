---
title: Ressourcentyp fileSecurityState
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: cbf535dd6b30387afbe361389fa6bcfca1fc68fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065337"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="9f6fa-104">Ressourcentyp fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="9f6fa-104">fileSecurityState resource type</span></span>

 > <span data-ttu-id="9f6fa-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9f6fa-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f6fa-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f6fa-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f6fa-107">Enthält Informationen zur Datei (nicht verarbeiten) im Zusammenhang mit der Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="9f6fa-107">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="9f6fa-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9f6fa-108">Properties</span></span>

| <span data-ttu-id="9f6fa-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9f6fa-109">Property</span></span>   | <span data-ttu-id="9f6fa-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9f6fa-110">Type</span></span>|<span data-ttu-id="9f6fa-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f6fa-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f6fa-112">fileHash</span><span class="sxs-lookup"><span data-stu-id="9f6fa-112">fileHash</span></span>|[<span data-ttu-id="9f6fa-113">fileHash</span><span class="sxs-lookup"><span data-stu-id="9f6fa-113">fileHash</span></span>](filehash.md)|<span data-ttu-id="9f6fa-114">Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="9f6fa-114">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="9f6fa-115">name</span><span class="sxs-lookup"><span data-stu-id="9f6fa-115">name</span></span>|<span data-ttu-id="9f6fa-116">String</span><span class="sxs-lookup"><span data-stu-id="9f6fa-116">String</span></span>|<span data-ttu-id="9f6fa-117">Der Dateiname (ohne Pfad).</span><span class="sxs-lookup"><span data-stu-id="9f6fa-117">File name (without path).</span></span>|
|<span data-ttu-id="9f6fa-118">Pfad</span><span class="sxs-lookup"><span data-stu-id="9f6fa-118">path</span></span>|<span data-ttu-id="9f6fa-119">String</span><span class="sxs-lookup"><span data-stu-id="9f6fa-119">String</span></span>|<span data-ttu-id="9f6fa-120">Vollständiger Dateipfad der die Datei/ImageFile.</span><span class="sxs-lookup"><span data-stu-id="9f6fa-120">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="9f6fa-121">riskScore</span><span class="sxs-lookup"><span data-stu-id="9f6fa-121">riskScore</span></span>|<span data-ttu-id="9f6fa-122">String</span><span class="sxs-lookup"><span data-stu-id="9f6fa-122">String</span></span>|<span data-ttu-id="9f6fa-123">Anbieter generiert/berechnet riskieren Bewertung der alert-Datei.</span><span class="sxs-lookup"><span data-stu-id="9f6fa-123">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="9f6fa-124">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="9f6fa-124">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f6fa-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9f6fa-125">JSON representation</span></span>

<span data-ttu-id="9f6fa-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9f6fa-126">The following is a JSON representation of the resource.</span></span>

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