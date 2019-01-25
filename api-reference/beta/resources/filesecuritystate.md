---
title: Ressourcentyp fileSecurityState
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 485addfda2707c8848c44c839f9593378943f327
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526956"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="ced9a-104">Ressourcentyp fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="ced9a-104">fileSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ced9a-105">Enthält Informationen zur Datei (nicht verarbeiten) im Zusammenhang mit der Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="ced9a-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="ced9a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ced9a-106">Properties</span></span>

| <span data-ttu-id="ced9a-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ced9a-107">Property</span></span>   | <span data-ttu-id="ced9a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ced9a-108">Type</span></span>|<span data-ttu-id="ced9a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ced9a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ced9a-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="ced9a-110">fileHash</span></span>|[<span data-ttu-id="ced9a-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="ced9a-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="ced9a-112">Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="ced9a-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="ced9a-113">name</span><span class="sxs-lookup"><span data-stu-id="ced9a-113">name</span></span>|<span data-ttu-id="ced9a-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ced9a-114">String</span></span>|<span data-ttu-id="ced9a-115">Der Dateiname (ohne Pfad).</span><span class="sxs-lookup"><span data-stu-id="ced9a-115">File name (without path).</span></span>|
|<span data-ttu-id="ced9a-116">Pfad</span><span class="sxs-lookup"><span data-stu-id="ced9a-116">path</span></span>|<span data-ttu-id="ced9a-117">String</span><span class="sxs-lookup"><span data-stu-id="ced9a-117">String</span></span>|<span data-ttu-id="ced9a-118">Vollständiger Dateipfad der die Datei/ImageFile.</span><span class="sxs-lookup"><span data-stu-id="ced9a-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="ced9a-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="ced9a-119">riskScore</span></span>|<span data-ttu-id="ced9a-120">String</span><span class="sxs-lookup"><span data-stu-id="ced9a-120">String</span></span>|<span data-ttu-id="ced9a-121">Anbieter generiert/berechnet riskieren Bewertung der alert-Datei.</span><span class="sxs-lookup"><span data-stu-id="ced9a-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="ced9a-122">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="ced9a-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ced9a-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ced9a-123">JSON representation</span></span>

<span data-ttu-id="ced9a-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ced9a-124">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filesecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
