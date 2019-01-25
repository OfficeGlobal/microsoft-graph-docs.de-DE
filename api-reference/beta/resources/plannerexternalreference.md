---
title: plannerExternalReference-Ressourcentyp
description: Die **plannerExternalReference**-Ressource stellt die Metadaten eines Verweises dar (Anlagen wie z. B. Datei, URL). Es ist der Wert von Eigenschaft-Wert-Paaren im externalReferences-Objekt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 95084e8a4d2d1b117fc627902b2bd8163fcc82f6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518709"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="50a3c-104">plannerExternalReference-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="50a3c-104">plannerExternalReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50a3c-p102">Die **plannerExternalReference**-Ressource stellt die Metadaten eines Verweises dar (Anlagen wie z. B. Datei, URL). Es ist der Wert von Eigenschaft-Wert-Paaren im [externalReferences](plannerexternalreferences.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="50a3c-p102">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="50a3c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="50a3c-107">Properties</span></span>
| <span data-ttu-id="50a3c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50a3c-108">Property</span></span>     | <span data-ttu-id="50a3c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="50a3c-109">Type</span></span>   |<span data-ttu-id="50a3c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50a3c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50a3c-111">Alias</span><span class="sxs-lookup"><span data-stu-id="50a3c-111">alias</span></span>|<span data-ttu-id="50a3c-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50a3c-112">String</span></span>|<span data-ttu-id="50a3c-113">Ein Namensalias zur Beschreibung des Verweises.</span><span class="sxs-lookup"><span data-stu-id="50a3c-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="50a3c-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="50a3c-114">lastModifiedBy</span></span>|[<span data-ttu-id="50a3c-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="50a3c-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="50a3c-p103">Schreibgeschützt. Benutzer-ID, von der das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="50a3c-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="50a3c-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50a3c-118">lastModifiedDateTime</span></span>|<span data-ttu-id="50a3c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50a3c-119">DateTimeOffset</span></span>|<span data-ttu-id="50a3c-p104">Schreibgeschützt. Datum und Uhrzeit der letzten Änderung des Objekts. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="50a3c-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="50a3c-124">previewPriority</span><span class="sxs-lookup"><span data-stu-id="50a3c-124">previewPriority</span></span>|<span data-ttu-id="50a3c-125">String</span><span class="sxs-lookup"><span data-stu-id="50a3c-125">String</span></span>|<span data-ttu-id="50a3c-126">Wird verwendet, um die relative Prioritätsreihenfolge festzulegen, in der der Verweis als Vorschau für die Aufgaben angezeigt wirdd.</span><span class="sxs-lookup"><span data-stu-id="50a3c-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="50a3c-127">type</span><span class="sxs-lookup"><span data-stu-id="50a3c-127">type</span></span>|<span data-ttu-id="50a3c-128">String</span><span class="sxs-lookup"><span data-stu-id="50a3c-128">String</span></span>|<span data-ttu-id="50a3c-p105">Wird verwendet, um den Verweis zu beschreiben. Zu den Typen gehören: `PowerPoint`, `Word`, `Excel`, `Other`.</span><span class="sxs-lookup"><span data-stu-id="50a3c-p105">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50a3c-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="50a3c-131">JSON representation</span></span>
<span data-ttu-id="50a3c-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="50a3c-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerexternalreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
