---
title: page-Ressourcentyp
description: Eine Seite in einem OneNote-Notizbuch.
localization_priority: Normal
ms.openlocfilehash: d8c27cdc144e9b192bd0205f256653ff7f04df5f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649415"
---
# <a name="page-resource-type"></a><span data-ttu-id="9c1d6-103">page-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9c1d6-103">page resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c1d6-104">Eine Seite in einem OneNote-Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c1d6-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9c1d6-105">JSON representation</span></span>

<span data-ttu-id="9c1d6-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="9c1d6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9c1d6-107">Properties</span></span>
| <span data-ttu-id="9c1d6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9c1d6-108">Property</span></span>     | <span data-ttu-id="9c1d6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9c1d6-109">Type</span></span>   |<span data-ttu-id="9c1d6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c1d6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c1d6-111">Inhalt</span><span class="sxs-lookup"><span data-stu-id="9c1d6-111">content</span></span>|<span data-ttu-id="9c1d6-112">Stream</span><span class="sxs-lookup"><span data-stu-id="9c1d6-112">Stream</span></span>|<span data-ttu-id="9c1d6-113">Der HTML-Inhalt der Seite.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-113">The page's HTML content.</span></span>|
|<span data-ttu-id="9c1d6-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="9c1d6-114">contentUrl</span></span>|<span data-ttu-id="9c1d6-115">String</span><span class="sxs-lookup"><span data-stu-id="9c1d6-115">String</span></span>|<span data-ttu-id="9c1d6-p101">Die URL für die HTML-Inhalt der Seite.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="9c1d6-118">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="9c1d6-118">createdByAppId</span></span>|<span data-ttu-id="9c1d6-119">String</span><span class="sxs-lookup"><span data-stu-id="9c1d6-119">String</span></span>|<span data-ttu-id="9c1d6-p102">Der eindeutige Bezeichner der Anwendung, mit der die Seite erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="9c1d6-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c1d6-122">createdDateTime</span></span>|<span data-ttu-id="9c1d6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c1d6-123">DateTimeOffset</span></span>|<span data-ttu-id="9c1d6-p103">Das Datum und die Uhrzeit der Erstellung der Seite. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="9c1d6-128">id</span><span class="sxs-lookup"><span data-stu-id="9c1d6-128">id</span></span>|<span data-ttu-id="9c1d6-129">String</span><span class="sxs-lookup"><span data-stu-id="9c1d6-129">String</span></span>|<span data-ttu-id="9c1d6-p104">Der eindeutige Bezeichner der Seite.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="9c1d6-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c1d6-132">lastModifiedDateTime</span></span>|<span data-ttu-id="9c1d6-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c1d6-133">DateTimeOffset</span></span>|<span data-ttu-id="9c1d6-p105">Das Datum und die Uhrzeit der letzten Änderung der Seite. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="9c1d6-138">Ebene</span><span class="sxs-lookup"><span data-stu-id="9c1d6-138">level</span></span>|<span data-ttu-id="9c1d6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="9c1d6-139">Int32</span></span>|<span data-ttu-id="9c1d6-p106">Die Einzugsebene der Seite. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="9c1d6-142">links</span><span class="sxs-lookup"><span data-stu-id="9c1d6-142">links</span></span>|[<span data-ttu-id="9c1d6-143">PageLinks</span><span class="sxs-lookup"><span data-stu-id="9c1d6-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="9c1d6-p107">Links zum Öffnen der Seite. Der Link `oneNoteClientURL` öffnet die Seite im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebUrl` öffnet die Seite in OneNote Online. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="9c1d6-148">order</span><span class="sxs-lookup"><span data-stu-id="9c1d6-148">order</span></span>|<span data-ttu-id="9c1d6-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9c1d6-149">Int32</span></span>|<span data-ttu-id="9c1d6-p108">Die Anordnung der Seite im übergeordneten Abschnitt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="9c1d6-152">self</span><span class="sxs-lookup"><span data-stu-id="9c1d6-152">self</span></span>|<span data-ttu-id="9c1d6-153">String</span><span class="sxs-lookup"><span data-stu-id="9c1d6-153">String</span></span>|<span data-ttu-id="9c1d6-p109">Der Endpunkt, an dem Sie Details zur Seite abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="9c1d6-156">title</span><span class="sxs-lookup"><span data-stu-id="9c1d6-156">title</span></span>|<span data-ttu-id="9c1d6-157">String</span><span class="sxs-lookup"><span data-stu-id="9c1d6-157">String</span></span>|<span data-ttu-id="9c1d6-158">Der Titel der Seite.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9c1d6-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9c1d6-159">Relationships</span></span>
| <span data-ttu-id="9c1d6-160">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9c1d6-160">Relationship</span></span> | <span data-ttu-id="9c1d6-161">Typ</span><span class="sxs-lookup"><span data-stu-id="9c1d6-161">Type</span></span>   |<span data-ttu-id="9c1d6-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c1d6-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c1d6-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="9c1d6-163">parentNotebook</span></span>|[<span data-ttu-id="9c1d6-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="9c1d6-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="9c1d6-p110">Das Notizbuch, das die Seite enthält.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="9c1d6-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="9c1d6-167">parentSection</span></span>|[<span data-ttu-id="9c1d6-168">Section</span><span class="sxs-lookup"><span data-stu-id="9c1d6-168">Section</span></span>](section.md)|<span data-ttu-id="9c1d6-p111">Der Abschnitt, der die Seite enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="9c1d6-171">Methoden</span><span class="sxs-lookup"><span data-stu-id="9c1d6-171">Methods</span></span>

| <span data-ttu-id="9c1d6-172">Methode</span><span class="sxs-lookup"><span data-stu-id="9c1d6-172">Method</span></span>           | <span data-ttu-id="9c1d6-173">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9c1d6-173">Return Type</span></span>    |<span data-ttu-id="9c1d6-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c1d6-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c1d6-175">Seite abrufen</span><span class="sxs-lookup"><span data-stu-id="9c1d6-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="9c1d6-176">Page</span><span class="sxs-lookup"><span data-stu-id="9c1d6-176">Page</span></span>](page.md) |<span data-ttu-id="9c1d6-177">Dient zum Lesen der Eigenschaften und Beziehungen der Seite.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="9c1d6-178">Seiteninhalt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9c1d6-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="9c1d6-179">Keine</span><span class="sxs-lookup"><span data-stu-id="9c1d6-179">None</span></span> |<span data-ttu-id="9c1d6-180">Dient zum Aktualisieren des HTML-Inhalts der Seite.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="9c1d6-181">Seite löschen</span><span class="sxs-lookup"><span data-stu-id="9c1d6-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="9c1d6-182">Keine</span><span class="sxs-lookup"><span data-stu-id="9c1d6-182">None</span></span> |<span data-ttu-id="9c1d6-183">Dient zum Löschen der Seite.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-183">Delete the page.</span></span> |
|[<span data-ttu-id="9c1d6-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="9c1d6-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="9c1d6-185">Keine</span><span class="sxs-lookup"><span data-stu-id="9c1d6-185">None</span></span> |<span data-ttu-id="9c1d6-186">Kopiert die Seite in einen bestimmten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="9c1d6-186">Copies the page to a specific section.</span></span>|

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
