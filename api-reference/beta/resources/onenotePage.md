---
title: page-Ressourcentyp
description: Eine Seite in einem OneNote-Notizbuch.
localization_priority: Normal
ms.openlocfilehash: 81ab6ea0bc7ac3e10f0ec369da1e587b5e9b808b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29579926"
---
# <a name="page-resource-type"></a><span data-ttu-id="2bc64-103">page-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2bc64-103">page resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bc64-104">Eine Seite in einem OneNote-Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="2bc64-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bc64-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2bc64-105">JSON representation</span></span>

<span data-ttu-id="2bc64-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2bc64-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a><span data-ttu-id="2bc64-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2bc64-107">Properties</span></span>
| <span data-ttu-id="2bc64-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2bc64-108">Property</span></span>     | <span data-ttu-id="2bc64-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2bc64-109">Type</span></span>   |<span data-ttu-id="2bc64-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2bc64-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bc64-111">Inhalt</span><span class="sxs-lookup"><span data-stu-id="2bc64-111">content</span></span>|<span data-ttu-id="2bc64-112">Stream</span><span class="sxs-lookup"><span data-stu-id="2bc64-112">Stream</span></span>|<span data-ttu-id="2bc64-113">Der HTML-Inhalt der Seite.</span><span class="sxs-lookup"><span data-stu-id="2bc64-113">The page's HTML content.</span></span>|
|<span data-ttu-id="2bc64-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="2bc64-114">contentUrl</span></span>|<span data-ttu-id="2bc64-115">String</span><span class="sxs-lookup"><span data-stu-id="2bc64-115">String</span></span>|<span data-ttu-id="2bc64-p101">Die URL für die HTML-Inhalt der Seite.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="2bc64-118">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="2bc64-118">createdByAppId</span></span>|<span data-ttu-id="2bc64-119">String</span><span class="sxs-lookup"><span data-stu-id="2bc64-119">String</span></span>|<span data-ttu-id="2bc64-p102">Der eindeutige Bezeichner der Anwendung, mit der die Seite erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="2bc64-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2bc64-122">createdDateTime</span></span>|<span data-ttu-id="2bc64-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bc64-123">DateTimeOffset</span></span>|<span data-ttu-id="2bc64-p103">Das Datum und die Uhrzeit der Erstellung der Seite. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2bc64-128">id</span><span class="sxs-lookup"><span data-stu-id="2bc64-128">id</span></span>|<span data-ttu-id="2bc64-129">String</span><span class="sxs-lookup"><span data-stu-id="2bc64-129">String</span></span>|<span data-ttu-id="2bc64-p104">Der eindeutige Bezeichner der Seite.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="2bc64-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bc64-132">lastModifiedDateTime</span></span>|<span data-ttu-id="2bc64-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bc64-133">DateTimeOffset</span></span>|<span data-ttu-id="2bc64-p105">Das Datum und die Uhrzeit der letzten Änderung der Seite. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2bc64-138">Ebene</span><span class="sxs-lookup"><span data-stu-id="2bc64-138">level</span></span>|<span data-ttu-id="2bc64-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2bc64-139">Int32</span></span>|<span data-ttu-id="2bc64-p106">Die Einzugsebene der Seite. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="2bc64-142">links</span><span class="sxs-lookup"><span data-stu-id="2bc64-142">links</span></span>|[<span data-ttu-id="2bc64-143">pageLinks</span><span class="sxs-lookup"><span data-stu-id="2bc64-143">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="2bc64-p107">Links zum Öffnen der Seite. Der Link `oneNoteClientURL` öffnet die Seite im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebUrl` öffnet die Seite in OneNote Online. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="2bc64-148">order</span><span class="sxs-lookup"><span data-stu-id="2bc64-148">order</span></span>|<span data-ttu-id="2bc64-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2bc64-149">Int32</span></span>|<span data-ttu-id="2bc64-p108">Die Anordnung der Seite im übergeordneten Abschnitt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="2bc64-152">self</span><span class="sxs-lookup"><span data-stu-id="2bc64-152">self</span></span>|<span data-ttu-id="2bc64-153">String</span><span class="sxs-lookup"><span data-stu-id="2bc64-153">String</span></span>|<span data-ttu-id="2bc64-p109">Der Endpunkt, an dem Sie Details zur Seite abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="2bc64-156">title</span><span class="sxs-lookup"><span data-stu-id="2bc64-156">title</span></span>|<span data-ttu-id="2bc64-157">String</span><span class="sxs-lookup"><span data-stu-id="2bc64-157">String</span></span>|<span data-ttu-id="2bc64-158">Der Titel der Seite.</span><span class="sxs-lookup"><span data-stu-id="2bc64-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2bc64-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2bc64-159">Relationships</span></span>
| <span data-ttu-id="2bc64-160">Beziehung</span><span class="sxs-lookup"><span data-stu-id="2bc64-160">Relationship</span></span> | <span data-ttu-id="2bc64-161">Typ</span><span class="sxs-lookup"><span data-stu-id="2bc64-161">Type</span></span>   |<span data-ttu-id="2bc64-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2bc64-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bc64-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="2bc64-163">parentNotebook</span></span>|[<span data-ttu-id="2bc64-164">Notizbuch</span><span class="sxs-lookup"><span data-stu-id="2bc64-164">notebook</span></span>](notebook.md)|<span data-ttu-id="2bc64-p110">Das Notizbuch, das die Seite enthält.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="2bc64-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="2bc64-167">parentSection</span></span>|[<span data-ttu-id="2bc64-168">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="2bc64-168">onenoteSection</span></span>](section.md)|<span data-ttu-id="2bc64-p111">Der Abschnitt, der die Seite enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="2bc64-171">Methoden</span><span class="sxs-lookup"><span data-stu-id="2bc64-171">Methods</span></span>

| <span data-ttu-id="2bc64-172">Methode</span><span class="sxs-lookup"><span data-stu-id="2bc64-172">Method</span></span>           | <span data-ttu-id="2bc64-173">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2bc64-173">Return Type</span></span>    |<span data-ttu-id="2bc64-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2bc64-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2bc64-175">Seite abrufen</span><span class="sxs-lookup"><span data-stu-id="2bc64-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="2bc64-176">onenotePage</span><span class="sxs-lookup"><span data-stu-id="2bc64-176">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="2bc64-177">Dient zum Lesen der Eigenschaften und Beziehungen der Seite.</span><span class="sxs-lookup"><span data-stu-id="2bc64-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="2bc64-178">Seiteninhalt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2bc64-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="2bc64-179">Keine</span><span class="sxs-lookup"><span data-stu-id="2bc64-179">None</span></span> |<span data-ttu-id="2bc64-180">Dient zum Aktualisieren des HTML-Inhalts der Seite.</span><span class="sxs-lookup"><span data-stu-id="2bc64-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="2bc64-181">Seite löschen</span><span class="sxs-lookup"><span data-stu-id="2bc64-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="2bc64-182">Keine</span><span class="sxs-lookup"><span data-stu-id="2bc64-182">None</span></span> |<span data-ttu-id="2bc64-183">Dient zum Löschen der Seite.</span><span class="sxs-lookup"><span data-stu-id="2bc64-183">Delete the page.</span></span> |
|[<span data-ttu-id="2bc64-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="2bc64-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="2bc64-185">Keine</span><span class="sxs-lookup"><span data-stu-id="2bc64-185">None</span></span> |<span data-ttu-id="2bc64-186">Kopiert die Seite in einen bestimmten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="2bc64-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/page.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
