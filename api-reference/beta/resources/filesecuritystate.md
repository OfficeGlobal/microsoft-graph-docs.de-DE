---
title: Ressourcentyp fileSecurityState
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 9d18021591b24d26577e41897111b90310746d18
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869503"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="54fde-104">Ressourcentyp fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="54fde-104">fileSecurityState resource type</span></span>

 > <span data-ttu-id="54fde-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="54fde-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54fde-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54fde-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54fde-107">Enthält Informationen zur Datei (nicht verarbeiten) im Zusammenhang mit der Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="54fde-107">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="54fde-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="54fde-108">Properties</span></span>

| <span data-ttu-id="54fde-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54fde-109">Property</span></span>   | <span data-ttu-id="54fde-110">Typ</span><span class="sxs-lookup"><span data-stu-id="54fde-110">Type</span></span>|<span data-ttu-id="54fde-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54fde-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54fde-112">fileHash</span><span class="sxs-lookup"><span data-stu-id="54fde-112">fileHash</span></span>|[<span data-ttu-id="54fde-113">fileHash</span><span class="sxs-lookup"><span data-stu-id="54fde-113">fileHash</span></span>](filehash.md)|<span data-ttu-id="54fde-114">Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="54fde-114">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="54fde-115">name</span><span class="sxs-lookup"><span data-stu-id="54fde-115">name</span></span>|<span data-ttu-id="54fde-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fde-116">String</span></span>|<span data-ttu-id="54fde-117">Der Dateiname (ohne Pfad).</span><span class="sxs-lookup"><span data-stu-id="54fde-117">File name (without path).</span></span>|
|<span data-ttu-id="54fde-118">Pfad</span><span class="sxs-lookup"><span data-stu-id="54fde-118">path</span></span>|<span data-ttu-id="54fde-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fde-119">String</span></span>|<span data-ttu-id="54fde-120">Vollständiger Dateipfad der die Datei/ImageFile.</span><span class="sxs-lookup"><span data-stu-id="54fde-120">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="54fde-121">riskScore</span><span class="sxs-lookup"><span data-stu-id="54fde-121">riskScore</span></span>|<span data-ttu-id="54fde-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54fde-122">String</span></span>|<span data-ttu-id="54fde-123">Anbieter generiert/berechnet riskieren Bewertung der alert-Datei.</span><span class="sxs-lookup"><span data-stu-id="54fde-123">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="54fde-124">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="54fde-124">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54fde-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="54fde-125">JSON representation</span></span>

<span data-ttu-id="54fde-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="54fde-126">The following is a JSON representation of the resource.</span></span>

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
