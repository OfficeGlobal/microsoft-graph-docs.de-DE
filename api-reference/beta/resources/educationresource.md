---
title: Ressourcentyp educationResource
description: Eine übergeordnete Klasse für alle Resource-Objekten im System. Eine Ressource ist eine **Zuordnung** und/oder **Übermittlung**, das das Learning-Objekt darstellt, das wird zugeordnet
localization_priority: Normal
ms.openlocfilehash: 0608f3c0fb84f05404032bed611f0af887e7bb67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827559"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="115e8-104">Ressourcentyp educationResource</span><span class="sxs-lookup"><span data-stu-id="115e8-104">educationResource resource type</span></span>

> <span data-ttu-id="115e8-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="115e8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="115e8-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="115e8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="115e8-107">Eine übergeordnete Klasse für alle Resource-Objekten im System.</span><span class="sxs-lookup"><span data-stu-id="115e8-107">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="115e8-108">Eine Ressource ist zugeordnet, mit einer **Zuordnung** und/oder **Übermittlung**, das das Learning-Objekt darstellt, das wird ausgegeben werden, oder übergeben.</span><span class="sxs-lookup"><span data-stu-id="115e8-108">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="115e8-109">Eine Ressource kann nicht direkt instanziiert werden. Sie müssen eine Unterklasse vornehmen, die den Typ der Ressource verwendeten darstellt.</span><span class="sxs-lookup"><span data-stu-id="115e8-109">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="115e8-110">Diese Ressource werden die allgemeinen Eigenschaften für alle Arten von Ressource gespeichert.</span><span class="sxs-lookup"><span data-stu-id="115e8-110">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="115e8-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="115e8-111">Properties</span></span>
| <span data-ttu-id="115e8-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="115e8-112">Property</span></span>     | <span data-ttu-id="115e8-113">Typ</span><span class="sxs-lookup"><span data-stu-id="115e8-113">Type</span></span>   |<span data-ttu-id="115e8-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="115e8-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="115e8-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="115e8-115">createdBy</span></span>|[<span data-ttu-id="115e8-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="115e8-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="115e8-117">Die die Ressource erstellt.</span><span class="sxs-lookup"><span data-stu-id="115e8-117">Who created the resource.</span></span>|
|<span data-ttu-id="115e8-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="115e8-118">createdDateTime</span></span>|<span data-ttu-id="115e8-119">-Zeitpunkt der Erstellung die Ressource.</span><span class="sxs-lookup"><span data-stu-id="115e8-119">Moment in time when the resource was created.</span></span>  <span data-ttu-id="115e8-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="115e8-120">DateTimeOffset</span></span>|<span data-ttu-id="115e8-p105">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="115e8-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="115e8-123">displayName</span><span class="sxs-lookup"><span data-stu-id="115e8-123">displayName</span></span>|<span data-ttu-id="115e8-124">String</span><span class="sxs-lookup"><span data-stu-id="115e8-124">String</span></span>|<span data-ttu-id="115e8-125">Der Anzeigename der Ressource.</span><span class="sxs-lookup"><span data-stu-id="115e8-125">Display name of resource.</span></span>|
|<span data-ttu-id="115e8-126">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="115e8-126">lastModifiedBy</span></span>|[<span data-ttu-id="115e8-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="115e8-127">identitySet</span></span>](identityset.md)|<span data-ttu-id="115e8-128">Wer war der letzte Benutzer, die Ressource zu ändern.</span><span class="sxs-lookup"><span data-stu-id="115e8-128">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="115e8-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="115e8-129">lastModifiedDateTime</span></span>|<span data-ttu-id="115e8-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="115e8-130">DateTimeOffset</span></span>|<span data-ttu-id="115e8-131">Zeitpunkt der Uhrzeit der letzten die Ressource Änderung.</span><span class="sxs-lookup"><span data-stu-id="115e8-131">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="115e8-132">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="115e8-132">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="115e8-133">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="115e8-133">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="115e8-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="115e8-134">JSON representation</span></span>

<span data-ttu-id="115e8-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="115e8-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
