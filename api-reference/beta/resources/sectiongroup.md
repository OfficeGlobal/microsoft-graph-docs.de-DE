---
title: sectionGroup-Ressourcentyp
description: Eine Abschnittsgruppe in einem OneNote-Notizbuch. Abschnittsgruppen können Abschnitte und Abschnittsgruppen enthalten.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 65e420d014add658a538deb42c01518cd94d611c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523708"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="06727-104">sectionGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="06727-104">sectionGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06727-p102">Eine Abschnittsgruppe in einem OneNote-Notizbuch. Abschnittsgruppen können Abschnitte und Abschnittsgruppen enthalten.</span><span class="sxs-lookup"><span data-stu-id="06727-p102">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="06727-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="06727-107">JSON representation</span></span>

<span data-ttu-id="06727-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="06727-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectiongroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="06727-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="06727-109">Properties</span></span>
| <span data-ttu-id="06727-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06727-110">Property</span></span>     | <span data-ttu-id="06727-111">Typ</span><span class="sxs-lookup"><span data-stu-id="06727-111">Type</span></span>   |<span data-ttu-id="06727-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06727-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06727-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="06727-113">createdBy</span></span>|[<span data-ttu-id="06727-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="06727-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="06727-p103">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06727-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="06727-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06727-117">createdDateTime</span></span>|<span data-ttu-id="06727-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06727-118">DateTimeOffset</span></span>|<span data-ttu-id="06727-p104">Das Datum und die Uhrzeit der Erstellung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06727-p104">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="06727-123">id</span><span class="sxs-lookup"><span data-stu-id="06727-123">id</span></span>|<span data-ttu-id="06727-124">string</span><span class="sxs-lookup"><span data-stu-id="06727-124">String</span></span>|<span data-ttu-id="06727-p105">Der eindeutige Bezeichner der Abschnittsgruppe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06727-p105">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="06727-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="06727-127">lastModifiedBy</span></span>|[<span data-ttu-id="06727-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="06727-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="06727-p106">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06727-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="06727-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06727-131">lastModifiedDateTime</span></span>|<span data-ttu-id="06727-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06727-132">DateTimeOffset</span></span>|<span data-ttu-id="06727-p107">Das Datum und die Uhrzeit der letzten Änderung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06727-p107">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="06727-137">displayName</span><span class="sxs-lookup"><span data-stu-id="06727-137">displayName</span></span>|<span data-ttu-id="06727-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06727-138">String</span></span>|<span data-ttu-id="06727-139">Der Name der Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="06727-139">The name of the section group.</span></span>|
|<span data-ttu-id="06727-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="06727-140">sectionGroupsUrl</span></span>|<span data-ttu-id="06727-141">String</span><span class="sxs-lookup"><span data-stu-id="06727-141">String</span></span>|<span data-ttu-id="06727-p108">Die URL für die Navigationseigenschaft `sectionGroups`, die alle Abschnittsgruppen in der Abschnittsgruppe zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06727-p108">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="06727-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="06727-144">sectionsUrl</span></span>|<span data-ttu-id="06727-145">String</span><span class="sxs-lookup"><span data-stu-id="06727-145">String</span></span>|<span data-ttu-id="06727-p109">Die URL für die Navigationseigenschaft `sections`, die alle Abschnitte in der Abschnittsgruppe zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06727-p109">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="06727-148">self</span><span class="sxs-lookup"><span data-stu-id="06727-148">self</span></span>|<span data-ttu-id="06727-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06727-149">String</span></span>|<span data-ttu-id="06727-p110">Der Endpunkt, an dem Sie Details zur Abschnittsgruppe abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06727-p110">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06727-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="06727-152">Relationships</span></span>
| <span data-ttu-id="06727-153">Beziehung</span><span class="sxs-lookup"><span data-stu-id="06727-153">Relationship</span></span> | <span data-ttu-id="06727-154">Typ</span><span class="sxs-lookup"><span data-stu-id="06727-154">Type</span></span>   |<span data-ttu-id="06727-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06727-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06727-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="06727-156">parentNotebook</span></span>|[<span data-ttu-id="06727-157">Notebook</span><span class="sxs-lookup"><span data-stu-id="06727-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="06727-p111">Das Notizbuch, das die Abschnittsgruppe enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06727-p111">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="06727-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="06727-160">parentSectionGroup</span></span>|[<span data-ttu-id="06727-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="06727-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="06727-p112">Die Abschnittsgruppe, die die Abschnittsgruppe enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06727-p112">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="06727-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="06727-164">sectionGroups</span></span>|<span data-ttu-id="06727-165">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06727-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="06727-p113">Die Abschnittsgruppen im Abschnitt. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="06727-p113">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="06727-169">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="06727-169">sections</span></span>|<span data-ttu-id="06727-170">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06727-170">[Section](section.md) collection</span></span>|<span data-ttu-id="06727-p114">Die Abschnitte in der Abschnittsgruppe. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="06727-p114">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="06727-174">Methoden</span><span class="sxs-lookup"><span data-stu-id="06727-174">Methods</span></span>

| <span data-ttu-id="06727-175">Methode</span><span class="sxs-lookup"><span data-stu-id="06727-175">Method</span></span>           | <span data-ttu-id="06727-176">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="06727-176">Return Type</span></span>    |<span data-ttu-id="06727-177">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06727-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06727-178">Abschnittsgruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="06727-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="06727-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="06727-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="06727-180">Dient zum Lesen der Eigenschaften und Beziehungen der Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="06727-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="06727-181">Abschnittsgruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="06727-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="06727-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="06727-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="06727-183">Dient zum Erstellen einer Abschnittsgruppe durch Veröffentlichung in der sectionGroups-Sammlung in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="06727-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="06727-184">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="06727-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="06727-185">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06727-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="06727-186">Dient zum Abrufen der Sammlung von Abschnittsgruppen in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="06727-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="06727-187">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="06727-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="06727-188">Section</span><span class="sxs-lookup"><span data-stu-id="06727-188">Section</span></span>](section.md)| <span data-ttu-id="06727-189">Dient zum Erstellen eines Abschnitts durch Veröffentlichung in der sections-Sammlung in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="06727-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="06727-190">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="06727-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="06727-191">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06727-191">[Section](section.md) collection</span></span>| <span data-ttu-id="06727-192">Dient zum Abrufen einer Sammlung von Abschnitten in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="06727-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sectiongroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
