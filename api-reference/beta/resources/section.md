---
title: section-Ressourcentyp
description: Ein Abschnitt in einem OneNote-Notizbuch. Abschnitte können Seiten enthalten.
localization_priority: Normal
ms.openlocfilehash: ea33cfae128a7ea796f3f14bd165210cbfec121d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574138"
---
# <a name="section-resource-type"></a><span data-ttu-id="3afd3-104">section-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3afd3-104">section resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3afd3-p102">Ein Abschnitt in einem OneNote-Notizbuch. Abschnitte können Seiten enthalten.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p102">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3afd3-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3afd3-107">JSON representation</span></span>

<span data-ttu-id="3afd3-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3afd3-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="3afd3-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3afd3-109">Properties</span></span>
| <span data-ttu-id="3afd3-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3afd3-110">Property</span></span>     | <span data-ttu-id="3afd3-111">Typ</span><span class="sxs-lookup"><span data-stu-id="3afd3-111">Type</span></span>   |<span data-ttu-id="3afd3-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3afd3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3afd3-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="3afd3-113">createdBy</span></span>|[<span data-ttu-id="3afd3-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="3afd3-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="3afd3-p103">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="3afd3-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3afd3-117">createdDateTime</span></span>|<span data-ttu-id="3afd3-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3afd3-118">DateTimeOffset</span></span>|<span data-ttu-id="3afd3-p104">Das Datum und die Uhrzeit der Erstellung des Abschnitts. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p104">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="3afd3-123">id</span><span class="sxs-lookup"><span data-stu-id="3afd3-123">id</span></span>|<span data-ttu-id="3afd3-124">String</span><span class="sxs-lookup"><span data-stu-id="3afd3-124">String</span></span>|<span data-ttu-id="3afd3-p105">Der eindeutige Bezeichner des Abschnitts.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p105">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="3afd3-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="3afd3-127">isDefault</span></span>|<span data-ttu-id="3afd3-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="3afd3-128">Boolean</span></span>|<span data-ttu-id="3afd3-p106">Gibt an, ob dies der Standardabschnitt des Benutzers ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p106">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="3afd3-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3afd3-131">lastModifiedBy</span></span>|[<span data-ttu-id="3afd3-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="3afd3-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="3afd3-p107">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="3afd3-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3afd3-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3afd3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3afd3-136">DateTimeOffset</span></span>|<span data-ttu-id="3afd3-p108">Das Datum und die Uhrzeit der letzten Änderung des Abschnitts. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p108">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="3afd3-141">links</span><span class="sxs-lookup"><span data-stu-id="3afd3-141">links</span></span>|[<span data-ttu-id="3afd3-142">sectionLinks</span><span class="sxs-lookup"><span data-stu-id="3afd3-142">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="3afd3-p109">Links zum Öffnen des Abschnitts. Der Link `oneNoteClientURL` öffnet den Abschnitt im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebURL` öffnet den Abschnitt in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p109">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="3afd3-146">displayName</span><span class="sxs-lookup"><span data-stu-id="3afd3-146">displayName</span></span>|<span data-ttu-id="3afd3-147">String</span><span class="sxs-lookup"><span data-stu-id="3afd3-147">String</span></span>|<span data-ttu-id="3afd3-148">Der Name des Abschnitts.</span><span class="sxs-lookup"><span data-stu-id="3afd3-148">The name of the section.</span></span> |
|<span data-ttu-id="3afd3-149">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="3afd3-149">pagesUrl</span></span>|<span data-ttu-id="3afd3-150">String</span><span class="sxs-lookup"><span data-stu-id="3afd3-150">String</span></span>|<span data-ttu-id="3afd3-p110">Der Endpunkt `pages`, an dem Sie Details für alle Seiten im Abschnitt abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p110">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="3afd3-153">self</span><span class="sxs-lookup"><span data-stu-id="3afd3-153">self</span></span>|<span data-ttu-id="3afd3-154">String</span><span class="sxs-lookup"><span data-stu-id="3afd3-154">String</span></span>|<span data-ttu-id="3afd3-p111">Der Endpunkt, an dem Sie Details zum Abschnitt abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p111">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3afd3-157">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3afd3-157">Relationships</span></span>
| <span data-ttu-id="3afd3-158">Beziehung</span><span class="sxs-lookup"><span data-stu-id="3afd3-158">Relationship</span></span> | <span data-ttu-id="3afd3-159">Typ</span><span class="sxs-lookup"><span data-stu-id="3afd3-159">Type</span></span>   |<span data-ttu-id="3afd3-160">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3afd3-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3afd3-161">pages</span><span class="sxs-lookup"><span data-stu-id="3afd3-161">pages</span></span>|<span data-ttu-id="3afd3-162">[OnenotePage](onenotepage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3afd3-162">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="3afd3-p112">Ruft die Sammlung von Seiten in dem Abschnitt ab.  Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p112">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="3afd3-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="3afd3-166">parentNotebook</span></span>|[<span data-ttu-id="3afd3-167">Notizbuch</span><span class="sxs-lookup"><span data-stu-id="3afd3-167">notebook</span></span>](notebook.md)|<span data-ttu-id="3afd3-p113">Das Notizbuch, das den Abschnitt enthält.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p113">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="3afd3-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="3afd3-170">parentSectionGroup</span></span>|[<span data-ttu-id="3afd3-171">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="3afd3-171">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="3afd3-p114">Die Abschnittsgruppe, die den Abschnitt enthält.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-p114">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="3afd3-174">Methoden</span><span class="sxs-lookup"><span data-stu-id="3afd3-174">Methods</span></span>

| <span data-ttu-id="3afd3-175">Methode</span><span class="sxs-lookup"><span data-stu-id="3afd3-175">Method</span></span>           | <span data-ttu-id="3afd3-176">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3afd3-176">Return Type</span></span>    |<span data-ttu-id="3afd3-177">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3afd3-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3afd3-178">Abschnitt abrufen</span><span class="sxs-lookup"><span data-stu-id="3afd3-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="3afd3-179">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="3afd3-179">onenoteSection</span></span>](section.md) |<span data-ttu-id="3afd3-180">Dient zum Lesen der Eigenschaften und Beziehungen des Abschnitts.</span><span class="sxs-lookup"><span data-stu-id="3afd3-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="3afd3-181">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="3afd3-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="3afd3-182">onenotePage</span><span class="sxs-lookup"><span data-stu-id="3afd3-182">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="3afd3-183">Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung im angegebenen Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="3afd3-184">Seiten auflisten</span><span class="sxs-lookup"><span data-stu-id="3afd3-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="3afd3-185">[OnenotePage](onenotepage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3afd3-185">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="3afd3-186">Dient zum Abrufen einer Sammlung von Seiten im angegebenen Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="3afd3-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="3afd3-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="3afd3-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="3afd3-188">Keine</span><span class="sxs-lookup"><span data-stu-id="3afd3-188">None</span></span>|<span data-ttu-id="3afd3-189">Dient zum Kopieren des Abschnitts in ein bestimmtes Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="3afd3-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="3afd3-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="3afd3-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="3afd3-191">Keine</span><span class="sxs-lookup"><span data-stu-id="3afd3-191">None</span></span>|<span data-ttu-id="3afd3-192">Dient zum Kopieren des Abschnitts in eine bestimmte Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="3afd3-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/section.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
