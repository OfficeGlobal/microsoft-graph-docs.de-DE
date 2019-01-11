---
title: section-Ressourcentyp
description: Ein Abschnitt in einem OneNote-Notizbuch. Abschnitte können Seiten enthalten.
localization_priority: Normal
ms.openlocfilehash: 181fa3399f13d0490d9cd7d4599d8208633107b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831855"
---
# <a name="section-resource-type"></a><span data-ttu-id="6b40d-104">section-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6b40d-104">section resource type</span></span>

> <span data-ttu-id="6b40d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6b40d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b40d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b40d-p103">Ein Abschnitt in einem OneNote-Notizbuch. Abschnitte können Seiten enthalten.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p103">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b40d-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6b40d-109">JSON representation</span></span>

<span data-ttu-id="6b40d-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6b40d-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="6b40d-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6b40d-111">Properties</span></span>
| <span data-ttu-id="6b40d-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b40d-112">Property</span></span>     | <span data-ttu-id="6b40d-113">Typ</span><span class="sxs-lookup"><span data-stu-id="6b40d-113">Type</span></span>   |<span data-ttu-id="6b40d-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b40d-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b40d-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="6b40d-115">createdBy</span></span>|[<span data-ttu-id="6b40d-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="6b40d-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="6b40d-p104">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="6b40d-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b40d-119">createdDateTime</span></span>|<span data-ttu-id="6b40d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b40d-120">DateTimeOffset</span></span>|<span data-ttu-id="6b40d-p105">Das Datum und die Uhrzeit der Erstellung des Abschnitts. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p105">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="6b40d-125">id</span><span class="sxs-lookup"><span data-stu-id="6b40d-125">id</span></span>|<span data-ttu-id="6b40d-126">String</span><span class="sxs-lookup"><span data-stu-id="6b40d-126">String</span></span>|<span data-ttu-id="6b40d-p106">Der eindeutige Bezeichner des Abschnitts.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p106">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="6b40d-129">isDefault</span><span class="sxs-lookup"><span data-stu-id="6b40d-129">isDefault</span></span>|<span data-ttu-id="6b40d-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b40d-130">Boolean</span></span>|<span data-ttu-id="6b40d-p107">Gibt an, ob dies der Standardabschnitt des Benutzers ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p107">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="6b40d-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6b40d-133">lastModifiedBy</span></span>|[<span data-ttu-id="6b40d-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="6b40d-134">identitySet</span></span>](identityset.md)|<span data-ttu-id="6b40d-p108">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p108">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="6b40d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b40d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6b40d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b40d-138">DateTimeOffset</span></span>|<span data-ttu-id="6b40d-p109">Das Datum und die Uhrzeit der letzten Änderung des Abschnitts. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p109">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="6b40d-143">links</span><span class="sxs-lookup"><span data-stu-id="6b40d-143">links</span></span>|[<span data-ttu-id="6b40d-144">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="6b40d-144">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="6b40d-p110">Links zum Öffnen des Abschnitts. Der Link `oneNoteClientURL` öffnet den Abschnitt im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebURL` öffnet den Abschnitt in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p110">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="6b40d-148">displayName</span><span class="sxs-lookup"><span data-stu-id="6b40d-148">displayName</span></span>|<span data-ttu-id="6b40d-149">String</span><span class="sxs-lookup"><span data-stu-id="6b40d-149">String</span></span>|<span data-ttu-id="6b40d-150">Der Name des Abschnitts.</span><span class="sxs-lookup"><span data-stu-id="6b40d-150">The name of the section.</span></span> |
|<span data-ttu-id="6b40d-151">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="6b40d-151">pagesUrl</span></span>|<span data-ttu-id="6b40d-152">String</span><span class="sxs-lookup"><span data-stu-id="6b40d-152">String</span></span>|<span data-ttu-id="6b40d-p111">Der Endpunkt `pages`, an dem Sie Details für alle Seiten im Abschnitt abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p111">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="6b40d-155">self</span><span class="sxs-lookup"><span data-stu-id="6b40d-155">self</span></span>|<span data-ttu-id="6b40d-156">String</span><span class="sxs-lookup"><span data-stu-id="6b40d-156">String</span></span>|<span data-ttu-id="6b40d-p112">Der Endpunkt, an dem Sie Details zum Abschnitt abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p112">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b40d-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6b40d-159">Relationships</span></span>
| <span data-ttu-id="6b40d-160">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6b40d-160">Relationship</span></span> | <span data-ttu-id="6b40d-161">Typ</span><span class="sxs-lookup"><span data-stu-id="6b40d-161">Type</span></span>   |<span data-ttu-id="6b40d-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b40d-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b40d-163">pages</span><span class="sxs-lookup"><span data-stu-id="6b40d-163">pages</span></span>|<span data-ttu-id="6b40d-164">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6b40d-164">[Page](page.md) collection</span></span>|<span data-ttu-id="6b40d-p113">Ruft die Sammlung von Seiten in dem Abschnitt ab.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p113">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="6b40d-168">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="6b40d-168">parentNotebook</span></span>|[<span data-ttu-id="6b40d-169">Notebook</span><span class="sxs-lookup"><span data-stu-id="6b40d-169">Notebook</span></span>](notebook.md)|<span data-ttu-id="6b40d-p114">Das Notizbuch, das den Abschnitt enthält.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p114">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="6b40d-172">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="6b40d-172">parentSectionGroup</span></span>|[<span data-ttu-id="6b40d-173">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="6b40d-173">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="6b40d-p115">Die Abschnittsgruppe, die den Abschnitt enthält.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p115">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="6b40d-176">Methoden</span><span class="sxs-lookup"><span data-stu-id="6b40d-176">Methods</span></span>

| <span data-ttu-id="6b40d-177">Methode</span><span class="sxs-lookup"><span data-stu-id="6b40d-177">Method</span></span>           | <span data-ttu-id="6b40d-178">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6b40d-178">Return Type</span></span>    |<span data-ttu-id="6b40d-179">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b40d-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6b40d-180">Abschnitt abrufen</span><span class="sxs-lookup"><span data-stu-id="6b40d-180">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="6b40d-181">Section</span><span class="sxs-lookup"><span data-stu-id="6b40d-181">Section</span></span>](section.md) |<span data-ttu-id="6b40d-182">Dient zum Lesen der Eigenschaften und Beziehungen des Abschnitts.</span><span class="sxs-lookup"><span data-stu-id="6b40d-182">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="6b40d-183">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="6b40d-183">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="6b40d-184">Page</span><span class="sxs-lookup"><span data-stu-id="6b40d-184">Page</span></span>](page.md)| <span data-ttu-id="6b40d-185">Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung im angegebenen Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-185">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="6b40d-186">Seiten auflisten</span><span class="sxs-lookup"><span data-stu-id="6b40d-186">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="6b40d-187">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6b40d-187">[Page](page.md) collection</span></span>| <span data-ttu-id="6b40d-188">Dient zum Abrufen einer Sammlung von Seiten im angegebenen Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="6b40d-188">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="6b40d-189">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="6b40d-189">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="6b40d-190">Keine</span><span class="sxs-lookup"><span data-stu-id="6b40d-190">None</span></span>|<span data-ttu-id="6b40d-191">Dient zum Kopieren des Abschnitts in ein bestimmtes Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="6b40d-191">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="6b40d-192">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="6b40d-192">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="6b40d-193">Keine</span><span class="sxs-lookup"><span data-stu-id="6b40d-193">None</span></span>|<span data-ttu-id="6b40d-194">Dient zum Kopieren des Abschnitts in eine bestimmte Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="6b40d-194">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
