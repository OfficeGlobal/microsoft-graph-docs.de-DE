---
title: sectionGroup-Ressourcentyp
description: Eine Abschnittsgruppe in einem OneNote-Notizbuch. Abschnittsgruppen können Abschnitte und Abschnittsgruppen enthalten.
localization_priority: Normal
ms.openlocfilehash: 9e955d91fa49642100694da66421665a0d67b3da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855426"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="b9fc4-104">sectionGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b9fc4-104">sectionGroup resource type</span></span>

> <span data-ttu-id="b9fc4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9fc4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9fc4-p103">Eine Abschnittsgruppe in einem OneNote-Notizbuch. Abschnittsgruppen können Abschnitte und Abschnittsgruppen enthalten.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p103">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9fc4-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b9fc4-109">JSON representation</span></span>

<span data-ttu-id="b9fc4-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="b9fc4-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b9fc4-111">Properties</span></span>
| <span data-ttu-id="b9fc4-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9fc4-112">Property</span></span>     | <span data-ttu-id="b9fc4-113">Typ</span><span class="sxs-lookup"><span data-stu-id="b9fc4-113">Type</span></span>   |<span data-ttu-id="b9fc4-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9fc4-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9fc4-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="b9fc4-115">createdBy</span></span>|[<span data-ttu-id="b9fc4-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="b9fc4-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="b9fc4-p104">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="b9fc4-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9fc4-119">createdDateTime</span></span>|<span data-ttu-id="b9fc4-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9fc4-120">DateTimeOffset</span></span>|<span data-ttu-id="b9fc4-p105">Das Datum und die Uhrzeit der Erstellung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p105">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="b9fc4-125">id</span><span class="sxs-lookup"><span data-stu-id="b9fc4-125">id</span></span>|<span data-ttu-id="b9fc4-126">String</span><span class="sxs-lookup"><span data-stu-id="b9fc4-126">String</span></span>|<span data-ttu-id="b9fc4-p106">Der eindeutige Bezeichner der Abschnittsgruppe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p106">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="b9fc4-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b9fc4-129">lastModifiedBy</span></span>|[<span data-ttu-id="b9fc4-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="b9fc4-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="b9fc4-p107">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="b9fc4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9fc4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b9fc4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9fc4-134">DateTimeOffset</span></span>|<span data-ttu-id="b9fc4-p108">Das Datum und die Uhrzeit der letzten Änderung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p108">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="b9fc4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b9fc4-139">displayName</span></span>|<span data-ttu-id="b9fc4-140">String</span><span class="sxs-lookup"><span data-stu-id="b9fc4-140">String</span></span>|<span data-ttu-id="b9fc4-141">Der Name der Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-141">The name of the section group.</span></span>|
|<span data-ttu-id="b9fc4-142">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="b9fc4-142">sectionGroupsUrl</span></span>|<span data-ttu-id="b9fc4-143">String</span><span class="sxs-lookup"><span data-stu-id="b9fc4-143">String</span></span>|<span data-ttu-id="b9fc4-p109">Die URL für die Navigationseigenschaft `sectionGroups`, die alle Abschnittsgruppen in der Abschnittsgruppe zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="b9fc4-146">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="b9fc4-146">sectionsUrl</span></span>|<span data-ttu-id="b9fc4-147">String</span><span class="sxs-lookup"><span data-stu-id="b9fc4-147">String</span></span>|<span data-ttu-id="b9fc4-p110">Die URL für die Navigationseigenschaft `sections`, die alle Abschnitte in der Abschnittsgruppe zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p110">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="b9fc4-150">self</span><span class="sxs-lookup"><span data-stu-id="b9fc4-150">self</span></span>|<span data-ttu-id="b9fc4-151">String</span><span class="sxs-lookup"><span data-stu-id="b9fc4-151">String</span></span>|<span data-ttu-id="b9fc4-p111">Der Endpunkt, an dem Sie Details zur Abschnittsgruppe abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p111">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9fc4-154">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b9fc4-154">Relationships</span></span>
| <span data-ttu-id="b9fc4-155">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b9fc4-155">Relationship</span></span> | <span data-ttu-id="b9fc4-156">Typ</span><span class="sxs-lookup"><span data-stu-id="b9fc4-156">Type</span></span>   |<span data-ttu-id="b9fc4-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9fc4-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9fc4-158">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="b9fc4-158">parentNotebook</span></span>|[<span data-ttu-id="b9fc4-159">Notebook</span><span class="sxs-lookup"><span data-stu-id="b9fc4-159">Notebook</span></span>](notebook.md)|<span data-ttu-id="b9fc4-p112">Das Notizbuch, das die Abschnittsgruppe enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p112">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="b9fc4-162">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="b9fc4-162">parentSectionGroup</span></span>|[<span data-ttu-id="b9fc4-163">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="b9fc4-163">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="b9fc4-p113">Die Abschnittsgruppe, die die Abschnittsgruppe enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p113">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="b9fc4-166">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="b9fc4-166">sectionGroups</span></span>|<span data-ttu-id="b9fc4-167">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b9fc4-167">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="b9fc4-p114">Die Abschnittsgruppen im Abschnitt. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p114">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b9fc4-171">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="b9fc4-171">sections</span></span>|<span data-ttu-id="b9fc4-172">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b9fc4-172">[Section](section.md) collection</span></span>|<span data-ttu-id="b9fc4-p115">Die Abschnitte in der Abschnittsgruppe. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-p115">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="b9fc4-176">Methoden</span><span class="sxs-lookup"><span data-stu-id="b9fc4-176">Methods</span></span>

| <span data-ttu-id="b9fc4-177">Methode</span><span class="sxs-lookup"><span data-stu-id="b9fc4-177">Method</span></span>           | <span data-ttu-id="b9fc4-178">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b9fc4-178">Return Type</span></span>    |<span data-ttu-id="b9fc4-179">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9fc4-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b9fc4-180">Abschnittsgruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="b9fc4-180">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="b9fc4-181">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="b9fc4-181">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="b9fc4-182">Dient zum Lesen der Eigenschaften und Beziehungen der Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-182">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="b9fc4-183">Abschnittsgruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="b9fc4-183">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="b9fc4-184">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="b9fc4-184">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="b9fc4-185">Dient zum Erstellen einer Abschnittsgruppe durch Veröffentlichung in der sectionGroups-Sammlung in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-185">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="b9fc4-186">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="b9fc4-186">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="b9fc4-187">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b9fc4-187">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="b9fc4-188">Dient zum Abrufen der Sammlung von Abschnittsgruppen in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-188">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="b9fc4-189">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="b9fc4-189">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="b9fc4-190">Section</span><span class="sxs-lookup"><span data-stu-id="b9fc4-190">Section</span></span>](section.md)| <span data-ttu-id="b9fc4-191">Dient zum Erstellen eines Abschnitts durch Veröffentlichung in der sections-Sammlung in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-191">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="b9fc4-192">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="b9fc4-192">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="b9fc4-193">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b9fc4-193">[Section](section.md) collection</span></span>| <span data-ttu-id="b9fc4-194">Dient zum Abrufen einer Sammlung von Abschnitten in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="b9fc4-194">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
