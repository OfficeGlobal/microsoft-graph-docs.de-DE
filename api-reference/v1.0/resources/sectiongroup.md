---
title: sectionGroup-Ressourcentyp
description: Eine Abschnittsgruppe in einem OneNote-Notizbuch. Abschnittsgruppen können Abschnitte und Abschnittsgruppen enthalten.
ms.openlocfilehash: 4714d0d163e9ddd01373f50bf38fa0971da0609b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018468"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="d355f-104">sectionGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d355f-104">sectionGroup resource type</span></span>

<span data-ttu-id="d355f-p102">Eine Abschnittsgruppe in einem OneNote-Notizbuch. Abschnittsgruppen können Abschnitte und Abschnittsgruppen enthalten.</span><span class="sxs-lookup"><span data-stu-id="d355f-p102">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d355f-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d355f-107">JSON representation</span></span>

<span data-ttu-id="d355f-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d355f-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectionGroup"
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
## <a name="properties"></a><span data-ttu-id="d355f-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d355f-109">Properties</span></span>
| <span data-ttu-id="d355f-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d355f-110">Property</span></span>     | <span data-ttu-id="d355f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="d355f-111">Type</span></span>   |<span data-ttu-id="d355f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d355f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d355f-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="d355f-113">createdBy</span></span>|[<span data-ttu-id="d355f-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="d355f-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="d355f-p103">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d355f-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="d355f-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d355f-117">createdDateTime</span></span>|<span data-ttu-id="d355f-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d355f-118">DateTimeOffset</span></span>|<span data-ttu-id="d355f-p104">Das Datum und die Uhrzeit der Erstellung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d355f-p104">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="d355f-123">id</span><span class="sxs-lookup"><span data-stu-id="d355f-123">id</span></span>|<span data-ttu-id="d355f-124">String</span><span class="sxs-lookup"><span data-stu-id="d355f-124">String</span></span>|<span data-ttu-id="d355f-p105">Der eindeutige Bezeichner der Abschnittsgruppe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d355f-p105">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="d355f-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d355f-127">lastModifiedBy</span></span>|[<span data-ttu-id="d355f-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="d355f-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="d355f-p106">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d355f-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="d355f-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d355f-131">lastModifiedDateTime</span></span>|<span data-ttu-id="d355f-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d355f-132">DateTimeOffset</span></span>|<span data-ttu-id="d355f-p107">Das Datum und die Uhrzeit der letzten Änderung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d355f-p107">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="d355f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d355f-137">displayName</span></span>|<span data-ttu-id="d355f-138">String</span><span class="sxs-lookup"><span data-stu-id="d355f-138">String</span></span>|<span data-ttu-id="d355f-139">Der Name der Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="d355f-139">The name of the section group.</span></span>|
|<span data-ttu-id="d355f-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="d355f-140">sectionGroupsUrl</span></span>|<span data-ttu-id="d355f-141">String</span><span class="sxs-lookup"><span data-stu-id="d355f-141">String</span></span>|<span data-ttu-id="d355f-p108">Die URL für die Navigationseigenschaft `sectionGroups`, die alle Abschnittsgruppen in der Abschnittsgruppe zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d355f-p108">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="d355f-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="d355f-144">sectionsUrl</span></span>|<span data-ttu-id="d355f-145">String</span><span class="sxs-lookup"><span data-stu-id="d355f-145">String</span></span>|<span data-ttu-id="d355f-p109">Die URL für die Navigationseigenschaft `sections`, die alle Abschnitte in der Abschnittsgruppe zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d355f-p109">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="d355f-148">self</span><span class="sxs-lookup"><span data-stu-id="d355f-148">self</span></span>|<span data-ttu-id="d355f-149">String</span><span class="sxs-lookup"><span data-stu-id="d355f-149">String</span></span>|<span data-ttu-id="d355f-p110">Der Endpunkt, an dem Sie Details zur Abschnittsgruppe abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d355f-p110">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d355f-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d355f-152">Relationships</span></span>
| <span data-ttu-id="d355f-153">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d355f-153">Relationship</span></span> | <span data-ttu-id="d355f-154">Typ</span><span class="sxs-lookup"><span data-stu-id="d355f-154">Type</span></span>   |<span data-ttu-id="d355f-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d355f-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d355f-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="d355f-156">parentNotebook</span></span>|[<span data-ttu-id="d355f-157">Notebook</span><span class="sxs-lookup"><span data-stu-id="d355f-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="d355f-p111">Das Notizbuch, das die Abschnittsgruppe enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d355f-p111">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="d355f-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="d355f-160">parentSectionGroup</span></span>|[<span data-ttu-id="d355f-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="d355f-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="d355f-p112">Die Abschnittsgruppe, die die Abschnittsgruppe enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d355f-p112">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="d355f-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="d355f-164">sectionGroups</span></span>|<span data-ttu-id="d355f-165">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d355f-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="d355f-p113">Die Abschnittsgruppen im Abschnitt. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="d355f-p113">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d355f-169">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="d355f-169">sections</span></span>|<span data-ttu-id="d355f-170">[OnenoteSection](section.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d355f-170">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="d355f-p114">Die Abschnitte in der Abschnittsgruppe. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="d355f-p114">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="d355f-174">Methoden</span><span class="sxs-lookup"><span data-stu-id="d355f-174">Methods</span></span>

| <span data-ttu-id="d355f-175">Methode</span><span class="sxs-lookup"><span data-stu-id="d355f-175">Method</span></span>           | <span data-ttu-id="d355f-176">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d355f-176">Return Type</span></span>    |<span data-ttu-id="d355f-177">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d355f-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d355f-178">Abschnittsgruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="d355f-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="d355f-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="d355f-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="d355f-180">Dient zum Lesen der Eigenschaften und Beziehungen der Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="d355f-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="d355f-181">Abschnittsgruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="d355f-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="d355f-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="d355f-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="d355f-183">Dient zum Erstellen einer Abschnittsgruppe durch Veröffentlichung in der sectionGroups-Sammlung in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="d355f-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="d355f-184">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="d355f-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="d355f-185">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d355f-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="d355f-186">Dient zum Abrufen der Sammlung von Abschnittsgruppen in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="d355f-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="d355f-187">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="d355f-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="d355f-188">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="d355f-188">OnenoteSection</span></span>](section.md)| <span data-ttu-id="d355f-189">Dient zum Erstellen eines Abschnitts durch Veröffentlichung in der sections-Sammlung in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="d355f-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="d355f-190">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="d355f-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="d355f-191">[OnenoteSection](section.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d355f-191">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="d355f-192">Dient zum Abrufen einer Sammlung von Abschnitten in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="d355f-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
