---
title: plannerExternalReference-Ressourcentyp
description: Die Ressource **PlannerExternalReference** stellt die Metadaten eines Verweises (Anlagen wie etwa URL-Datei). Es ist der Wert der Eigenschaft-Wert-Paare im ExternalReferences-Objekt.
localization_priority: Normal
ms.openlocfilehash: 104fd17698d57339de5c0d7a2ec4c5f42b254f49
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833779"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="e4cf7-104">plannerExternalReference-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e4cf7-104">plannerExternalReference resource type</span></span>

> <span data-ttu-id="e4cf7-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e4cf7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4cf7-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4cf7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4cf7-p103">Die **plannerExternalReference**-Ressource stellt die Metadaten eines Verweises dar (Anlagen wie z. B. Datei, URL). Es ist der Wert von Eigenschaft-Wert-Paaren im [externalReferences](plannerexternalreferences.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="e4cf7-p103">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="e4cf7-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e4cf7-109">Properties</span></span>
| <span data-ttu-id="e4cf7-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4cf7-110">Property</span></span>     | <span data-ttu-id="e4cf7-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e4cf7-111">Type</span></span>   |<span data-ttu-id="e4cf7-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4cf7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4cf7-113">Alias</span><span class="sxs-lookup"><span data-stu-id="e4cf7-113">alias</span></span>|<span data-ttu-id="e4cf7-114">String</span><span class="sxs-lookup"><span data-stu-id="e4cf7-114">String</span></span>|<span data-ttu-id="e4cf7-115">Ein Namensalias zur Beschreibung des Verweises.</span><span class="sxs-lookup"><span data-stu-id="e4cf7-115">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="e4cf7-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e4cf7-116">lastModifiedBy</span></span>|[<span data-ttu-id="e4cf7-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="e4cf7-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="e4cf7-p104">Schreibgeschützt. Benutzer-ID, von der das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="e4cf7-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="e4cf7-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4cf7-120">lastModifiedDateTime</span></span>|<span data-ttu-id="e4cf7-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4cf7-121">DateTimeOffset</span></span>|<span data-ttu-id="e4cf7-p105">Schreibgeschützt. Datum und Uhrzeit der letzten Änderung des Objekts. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e4cf7-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e4cf7-126">previewPriority</span><span class="sxs-lookup"><span data-stu-id="e4cf7-126">previewPriority</span></span>|<span data-ttu-id="e4cf7-127">String</span><span class="sxs-lookup"><span data-stu-id="e4cf7-127">String</span></span>|<span data-ttu-id="e4cf7-128">Wird verwendet, um die relative Prioritätsreihenfolge festzulegen, in der der Verweis als Vorschau für die Aufgaben angezeigt wirdd.</span><span class="sxs-lookup"><span data-stu-id="e4cf7-128">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="e4cf7-129">type</span><span class="sxs-lookup"><span data-stu-id="e4cf7-129">type</span></span>|<span data-ttu-id="e4cf7-130">String</span><span class="sxs-lookup"><span data-stu-id="e4cf7-130">String</span></span>|<span data-ttu-id="e4cf7-p106">Wird verwendet, um den Verweis zu beschreiben. Zu den Typen gehören: `PowerPoint`, `Word`, `Excel`, `Other`.</span><span class="sxs-lookup"><span data-stu-id="e4cf7-p106">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4cf7-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e4cf7-133">JSON representation</span></span>
<span data-ttu-id="e4cf7-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e4cf7-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
