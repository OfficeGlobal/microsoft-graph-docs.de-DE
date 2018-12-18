---
title: Ressourcentyp sharingDetail
description: 'Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält. '
author: simonhult
ms.openlocfilehash: 8454fd451f0659ff3ccad270df3414a850bee180
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353375"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="57a72-103">Ressourcentyp sharingDetail</span><span class="sxs-lookup"><span data-stu-id="57a72-103">sharingDetail resource type</span></span>

> <span data-ttu-id="57a72-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="57a72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57a72-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="57a72-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="57a72-106">Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält.</span><span class="sxs-lookup"><span data-stu-id="57a72-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="57a72-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="57a72-107">JSON representation</span></span>
<span data-ttu-id="57a72-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="57a72-108">Here is a JSON representation of the resource</span></span>

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="57a72-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="57a72-109">Properties</span></span>

| <span data-ttu-id="57a72-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="57a72-110">Property</span></span>              | <span data-ttu-id="57a72-111">Typ</span><span class="sxs-lookup"><span data-stu-id="57a72-111">Type</span></span>          | <span data-ttu-id="57a72-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57a72-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="57a72-113">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="57a72-113">sharedDateTime</span></span>        | <span data-ttu-id="57a72-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57a72-114">DateTimeOffset</span></span>| <span data-ttu-id="57a72-115">Das Datum und die Zeit, die die Datei zuletzt freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="57a72-115">The date and time the file was last shared.</span></span> <span data-ttu-id="57a72-116">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="57a72-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="57a72-117">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="57a72-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="57a72-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="57a72-118">Read-only.</span></span>  |
| <span data-ttu-id="57a72-119">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="57a72-119">sharingSubject</span></span>        | <span data-ttu-id="57a72-120">String</span><span class="sxs-lookup"><span data-stu-id="57a72-120">String</span></span>          | <span data-ttu-id="57a72-121">Der Betreff, mit dem das Dokument freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="57a72-121">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="57a72-122">sharingType</span><span class="sxs-lookup"><span data-stu-id="57a72-122">sharingType</span></span>             | <span data-ttu-id="57a72-123">String</span><span class="sxs-lookup"><span data-stu-id="57a72-123">String</span></span>        | <span data-ttu-id="57a72-124">Bestimmt, wie das Dokument freigegeben wurde, kann durch "Link", "Anlage", "Group", "Site" sein.</span><span class="sxs-lookup"><span data-stu-id="57a72-124">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="57a72-125">sharedBy</span><span class="sxs-lookup"><span data-stu-id="57a72-125">sharedBy</span></span>                | [<span data-ttu-id="57a72-126">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="57a72-126">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="57a72-127">Der Benutzer, die das Dokument freigegeben.</span><span class="sxs-lookup"><span data-stu-id="57a72-127">The user who shared the document.</span></span>  |
| <span data-ttu-id="57a72-128">sharingReference</span><span class="sxs-lookup"><span data-stu-id="57a72-128">sharingReference</span></span>        | [<span data-ttu-id="57a72-129">resourceReference</span><span class="sxs-lookup"><span data-stu-id="57a72-129">resourceReference</span></span>](insights-resourcereference.md)      |  |