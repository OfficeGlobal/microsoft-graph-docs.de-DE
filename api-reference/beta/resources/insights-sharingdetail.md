---
title: Ressourcentyp sharingDetail
description: 'Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält. '
ms.openlocfilehash: 5ea54c9b8622c9f302609c6fbe299b9b68720793
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061764"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="3d5ba-103">Ressourcentyp sharingDetail</span><span class="sxs-lookup"><span data-stu-id="3d5ba-103">sharingDetail resource type</span></span>

> <span data-ttu-id="3d5ba-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3d5ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d5ba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d5ba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d5ba-106">Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält.</span><span class="sxs-lookup"><span data-stu-id="3d5ba-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="3d5ba-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3d5ba-107">JSON representation</span></span>
<span data-ttu-id="3d5ba-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3d5ba-108">Here is a JSON representation of the resource</span></span>

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="3d5ba-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3d5ba-109">Properties</span></span>

| <span data-ttu-id="3d5ba-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d5ba-110">Property</span></span>              | <span data-ttu-id="3d5ba-111">Typ</span><span class="sxs-lookup"><span data-stu-id="3d5ba-111">Type</span></span>          | <span data-ttu-id="3d5ba-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d5ba-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="3d5ba-113">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d5ba-113">sharedDateTime</span></span>        | <span data-ttu-id="3d5ba-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d5ba-114">DateTimeOffset</span></span>| <span data-ttu-id="3d5ba-115">Das Datum und die Zeit, die die Datei zuletzt freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="3d5ba-115">The date and time the file was last shared.</span></span> <span data-ttu-id="3d5ba-116">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="3d5ba-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3d5ba-117">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="3d5ba-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="3d5ba-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3d5ba-118">Read-only.</span></span>  |
| <span data-ttu-id="3d5ba-119">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="3d5ba-119">sharingSubject</span></span>        | <span data-ttu-id="3d5ba-120">String</span><span class="sxs-lookup"><span data-stu-id="3d5ba-120">String</span></span>          | <span data-ttu-id="3d5ba-121">Der Betreff, mit dem das Dokument freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="3d5ba-121">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="3d5ba-122">sharingType</span><span class="sxs-lookup"><span data-stu-id="3d5ba-122">sharingType</span></span>             | <span data-ttu-id="3d5ba-123">String</span><span class="sxs-lookup"><span data-stu-id="3d5ba-123">String</span></span>        | <span data-ttu-id="3d5ba-124">Bestimmt, wie das Dokument freigegeben wurde, kann durch "Link", "Anlage", "Group", "Site" sein.</span><span class="sxs-lookup"><span data-stu-id="3d5ba-124">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="3d5ba-125">sharedBy</span><span class="sxs-lookup"><span data-stu-id="3d5ba-125">sharedBy</span></span>                | [<span data-ttu-id="3d5ba-126">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="3d5ba-126">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="3d5ba-127">Der Benutzer, die das Dokument freigegeben.</span><span class="sxs-lookup"><span data-stu-id="3d5ba-127">The user who shared the document.</span></span>  |
| <span data-ttu-id="3d5ba-128">sharingReference</span><span class="sxs-lookup"><span data-stu-id="3d5ba-128">sharingReference</span></span>        | [<span data-ttu-id="3d5ba-129">resourceReference</span><span class="sxs-lookup"><span data-stu-id="3d5ba-129">resourceReference</span></span>](insights-resourcereference.md)      |  |