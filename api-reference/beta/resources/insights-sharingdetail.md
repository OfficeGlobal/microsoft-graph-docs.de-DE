---
title: Ressourcentyp sharingDetail
description: 'Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält. '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 3fff669b2b337e9566cd41a7cd5eb5ab73a84944
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512269"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="71bae-103">Ressourcentyp sharingDetail</span><span class="sxs-lookup"><span data-stu-id="71bae-103">sharingDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71bae-104">Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält.</span><span class="sxs-lookup"><span data-stu-id="71bae-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="71bae-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71bae-105">JSON representation</span></span>
<span data-ttu-id="71bae-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71bae-106">Here is a JSON representation of the resource</span></span>

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="71bae-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71bae-107">Properties</span></span>

| <span data-ttu-id="71bae-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71bae-108">Property</span></span>              | <span data-ttu-id="71bae-109">Typ</span><span class="sxs-lookup"><span data-stu-id="71bae-109">Type</span></span>          | <span data-ttu-id="71bae-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71bae-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="71bae-111">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="71bae-111">sharedDateTime</span></span>        | <span data-ttu-id="71bae-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71bae-112">DateTimeOffset</span></span>| <span data-ttu-id="71bae-113">Das Datum und die Zeit, die die Datei zuletzt freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="71bae-113">The date and time the file was last shared.</span></span> <span data-ttu-id="71bae-114">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="71bae-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="71bae-115">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="71bae-115">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="71bae-116">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71bae-116">Read-only.</span></span>  |
| <span data-ttu-id="71bae-117">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="71bae-117">sharingSubject</span></span>        | <span data-ttu-id="71bae-118">String</span><span class="sxs-lookup"><span data-stu-id="71bae-118">String</span></span>          | <span data-ttu-id="71bae-119">Der Betreff, mit dem das Dokument freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="71bae-119">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="71bae-120">SharingType</span><span class="sxs-lookup"><span data-stu-id="71bae-120">sharingType</span></span>             | <span data-ttu-id="71bae-121">String</span><span class="sxs-lookup"><span data-stu-id="71bae-121">String</span></span>        | <span data-ttu-id="71bae-122">Bestimmt, wie das Dokument freigegeben wurde, kann durch "Link", "Anlage", "Group", "Site" sein.</span><span class="sxs-lookup"><span data-stu-id="71bae-122">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="71bae-123">sharedBy</span><span class="sxs-lookup"><span data-stu-id="71bae-123">sharedBy</span></span>                | [<span data-ttu-id="71bae-124">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="71bae-124">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="71bae-125">Der Benutzer, die das Dokument freigegeben.</span><span class="sxs-lookup"><span data-stu-id="71bae-125">The user who shared the document.</span></span>  |
| <span data-ttu-id="71bae-126">sharingReference</span><span class="sxs-lookup"><span data-stu-id="71bae-126">sharingReference</span></span>        | [<span data-ttu-id="71bae-127">resourceReference</span><span class="sxs-lookup"><span data-stu-id="71bae-127">resourceReference</span></span>](insights-resourcereference.md)      |  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-sharingdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
