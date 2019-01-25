---
title: Ressourcentyp educationResource
description: Eine übergeordnete Klasse für alle Resource-Objekten im System. Eine Ressource ist eine **Zuordnung** und/oder **Übermittlung**, das das Learning-Objekt darstellt, das wird zugeordnet
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 87b19f849e24f1780a1d13c7aa1b3eb83543fdec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523218"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="13e96-104">Ressourcentyp educationResource</span><span class="sxs-lookup"><span data-stu-id="13e96-104">educationResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13e96-105">Eine übergeordnete Klasse für alle Resource-Objekten im System.</span><span class="sxs-lookup"><span data-stu-id="13e96-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="13e96-106">Eine Ressource ist zugeordnet, mit einer **Zuordnung** und/oder **Übermittlung**, das das Learning-Objekt darstellt, das wird ausgegeben werden, oder übergeben.</span><span class="sxs-lookup"><span data-stu-id="13e96-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="13e96-107">Eine Ressource kann nicht direkt instanziiert werden. Sie müssen eine Unterklasse vornehmen, die den Typ der Ressource verwendeten darstellt.</span><span class="sxs-lookup"><span data-stu-id="13e96-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="13e96-108">Diese Ressource werden die allgemeinen Eigenschaften für alle Arten von Ressource gespeichert.</span><span class="sxs-lookup"><span data-stu-id="13e96-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="13e96-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="13e96-109">Properties</span></span>
| <span data-ttu-id="13e96-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13e96-110">Property</span></span>     | <span data-ttu-id="13e96-111">Typ</span><span class="sxs-lookup"><span data-stu-id="13e96-111">Type</span></span>   |<span data-ttu-id="13e96-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13e96-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13e96-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="13e96-113">createdBy</span></span>|[<span data-ttu-id="13e96-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="13e96-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="13e96-115">Die die Ressource erstellt.</span><span class="sxs-lookup"><span data-stu-id="13e96-115">Who created the resource.</span></span>|
|<span data-ttu-id="13e96-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13e96-116">createdDateTime</span></span>|<span data-ttu-id="13e96-117">-Zeitpunkt der Erstellung die Ressource.</span><span class="sxs-lookup"><span data-stu-id="13e96-117">Moment in time when the resource was created.</span></span>  <span data-ttu-id="13e96-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13e96-118">DateTimeOffset</span></span>|<span data-ttu-id="13e96-p104">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="13e96-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="13e96-121">displayName</span><span class="sxs-lookup"><span data-stu-id="13e96-121">displayName</span></span>|<span data-ttu-id="13e96-122">String</span><span class="sxs-lookup"><span data-stu-id="13e96-122">String</span></span>|<span data-ttu-id="13e96-123">Der Anzeigename der Ressource.</span><span class="sxs-lookup"><span data-stu-id="13e96-123">Display name of resource.</span></span>|
|<span data-ttu-id="13e96-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="13e96-124">lastModifiedBy</span></span>|[<span data-ttu-id="13e96-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="13e96-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="13e96-126">Wer war der letzte Benutzer, die Ressource zu ändern.</span><span class="sxs-lookup"><span data-stu-id="13e96-126">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="13e96-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13e96-127">lastModifiedDateTime</span></span>|<span data-ttu-id="13e96-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13e96-128">DateTimeOffset</span></span>|<span data-ttu-id="13e96-129">Zeitpunkt der Uhrzeit der letzten die Ressource Änderung.</span><span class="sxs-lookup"><span data-stu-id="13e96-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="13e96-130">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="13e96-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="13e96-131">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="13e96-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13e96-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="13e96-132">JSON representation</span></span>

<span data-ttu-id="13e96-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="13e96-133">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
