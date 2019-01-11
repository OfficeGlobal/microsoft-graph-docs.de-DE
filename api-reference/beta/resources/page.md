---
title: page-Ressourcentyp
description: Eine Seite in einem OneNote-Notizbuch.
localization_priority: Normal
ms.openlocfilehash: 5928f430fcbfe9f41c6aa83e99d7dfe737e8e1c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850134"
---
# <a name="page-resource-type"></a><span data-ttu-id="fd4a3-103">page-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fd4a3-103">page resource type</span></span>

> <span data-ttu-id="fd4a3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd4a3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd4a3-106">Eine Seite in einem OneNote-Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-106">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd4a3-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fd4a3-107">JSON representation</span></span>

<span data-ttu-id="fd4a3-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="fd4a3-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd4a3-109">Properties</span></span>
| <span data-ttu-id="fd4a3-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd4a3-110">Property</span></span>     | <span data-ttu-id="fd4a3-111">Typ</span><span class="sxs-lookup"><span data-stu-id="fd4a3-111">Type</span></span>   |<span data-ttu-id="fd4a3-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd4a3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd4a3-113">Inhalt</span><span class="sxs-lookup"><span data-stu-id="fd4a3-113">content</span></span>|<span data-ttu-id="fd4a3-114">Stream</span><span class="sxs-lookup"><span data-stu-id="fd4a3-114">Stream</span></span>|<span data-ttu-id="fd4a3-115">Der HTML-Inhalt der Seite.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-115">The page's HTML content.</span></span>|
|<span data-ttu-id="fd4a3-116">contentUrl</span><span class="sxs-lookup"><span data-stu-id="fd4a3-116">contentUrl</span></span>|<span data-ttu-id="fd4a3-117">String</span><span class="sxs-lookup"><span data-stu-id="fd4a3-117">String</span></span>|<span data-ttu-id="fd4a3-p102">Die URL für die HTML-Inhalt der Seite.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-p102">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="fd4a3-120">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="fd4a3-120">createdByAppId</span></span>|<span data-ttu-id="fd4a3-121">String</span><span class="sxs-lookup"><span data-stu-id="fd4a3-121">String</span></span>|<span data-ttu-id="fd4a3-p103">Der eindeutige Bezeichner der Anwendung, mit der die Seite erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-p103">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="fd4a3-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd4a3-124">createdDateTime</span></span>|<span data-ttu-id="fd4a3-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd4a3-125">DateTimeOffset</span></span>|<span data-ttu-id="fd4a3-p104">Das Datum und die Uhrzeit der Erstellung der Seite. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-p104">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="fd4a3-130">id</span><span class="sxs-lookup"><span data-stu-id="fd4a3-130">id</span></span>|<span data-ttu-id="fd4a3-131">String</span><span class="sxs-lookup"><span data-stu-id="fd4a3-131">String</span></span>|<span data-ttu-id="fd4a3-p105">Der eindeutige Bezeichner der Seite.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-p105">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="fd4a3-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd4a3-134">lastModifiedDateTime</span></span>|<span data-ttu-id="fd4a3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd4a3-135">DateTimeOffset</span></span>|<span data-ttu-id="fd4a3-p106">Das Datum und die Uhrzeit der letzten Änderung der Seite. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-p106">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="fd4a3-140">Ebene</span><span class="sxs-lookup"><span data-stu-id="fd4a3-140">level</span></span>|<span data-ttu-id="fd4a3-141">Int32</span><span class="sxs-lookup"><span data-stu-id="fd4a3-141">Int32</span></span>|<span data-ttu-id="fd4a3-p107">Die Einzugsebene der Seite. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-p107">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="fd4a3-144">links</span><span class="sxs-lookup"><span data-stu-id="fd4a3-144">links</span></span>|[<span data-ttu-id="fd4a3-145">PageLinks</span><span class="sxs-lookup"><span data-stu-id="fd4a3-145">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="fd4a3-p108">Links zum Öffnen der Seite. Der Link `oneNoteClientURL` öffnet die Seite im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebUrl` öffnet die Seite in OneNote Online. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-p108">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="fd4a3-150">order</span><span class="sxs-lookup"><span data-stu-id="fd4a3-150">order</span></span>|<span data-ttu-id="fd4a3-151">Int32</span><span class="sxs-lookup"><span data-stu-id="fd4a3-151">Int32</span></span>|<span data-ttu-id="fd4a3-p109">Die Anordnung der Seite im übergeordneten Abschnitt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-p109">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="fd4a3-154">self</span><span class="sxs-lookup"><span data-stu-id="fd4a3-154">self</span></span>|<span data-ttu-id="fd4a3-155">String</span><span class="sxs-lookup"><span data-stu-id="fd4a3-155">String</span></span>|<span data-ttu-id="fd4a3-p110">Der Endpunkt, an dem Sie Details zur Seite abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-p110">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="fd4a3-158">title</span><span class="sxs-lookup"><span data-stu-id="fd4a3-158">title</span></span>|<span data-ttu-id="fd4a3-159">String</span><span class="sxs-lookup"><span data-stu-id="fd4a3-159">String</span></span>|<span data-ttu-id="fd4a3-160">Der Titel der Seite.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-160">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fd4a3-161">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fd4a3-161">Relationships</span></span>
| <span data-ttu-id="fd4a3-162">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fd4a3-162">Relationship</span></span> | <span data-ttu-id="fd4a3-163">Typ</span><span class="sxs-lookup"><span data-stu-id="fd4a3-163">Type</span></span>   |<span data-ttu-id="fd4a3-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd4a3-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd4a3-165">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="fd4a3-165">parentNotebook</span></span>|[<span data-ttu-id="fd4a3-166">Notebook</span><span class="sxs-lookup"><span data-stu-id="fd4a3-166">Notebook</span></span>](notebook.md)|<span data-ttu-id="fd4a3-p111">Das Notizbuch, das die Seite enthält.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-p111">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="fd4a3-169">parentSection</span><span class="sxs-lookup"><span data-stu-id="fd4a3-169">parentSection</span></span>|[<span data-ttu-id="fd4a3-170">Section</span><span class="sxs-lookup"><span data-stu-id="fd4a3-170">Section</span></span>](section.md)|<span data-ttu-id="fd4a3-p112">Der Abschnitt, der die Seite enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-p112">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="fd4a3-173">Methoden</span><span class="sxs-lookup"><span data-stu-id="fd4a3-173">Methods</span></span>

| <span data-ttu-id="fd4a3-174">Methode</span><span class="sxs-lookup"><span data-stu-id="fd4a3-174">Method</span></span>           | <span data-ttu-id="fd4a3-175">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fd4a3-175">Return Type</span></span>    |<span data-ttu-id="fd4a3-176">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd4a3-176">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd4a3-177">Seite abrufen</span><span class="sxs-lookup"><span data-stu-id="fd4a3-177">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="fd4a3-178">Page</span><span class="sxs-lookup"><span data-stu-id="fd4a3-178">Page</span></span>](page.md) |<span data-ttu-id="fd4a3-179">Dient zum Lesen der Eigenschaften und Beziehungen der Seite.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-179">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="fd4a3-180">Seiteninhalt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fd4a3-180">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="fd4a3-181">Keine</span><span class="sxs-lookup"><span data-stu-id="fd4a3-181">None</span></span> |<span data-ttu-id="fd4a3-182">Dient zum Aktualisieren des HTML-Inhalts der Seite.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-182">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="fd4a3-183">Seite löschen</span><span class="sxs-lookup"><span data-stu-id="fd4a3-183">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="fd4a3-184">Keine</span><span class="sxs-lookup"><span data-stu-id="fd4a3-184">None</span></span> |<span data-ttu-id="fd4a3-185">Dient zum Löschen der Seite.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-185">Delete the page.</span></span> |
|[<span data-ttu-id="fd4a3-186">copyToSection</span><span class="sxs-lookup"><span data-stu-id="fd4a3-186">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="fd4a3-187">Keine</span><span class="sxs-lookup"><span data-stu-id="fd4a3-187">None</span></span> |<span data-ttu-id="fd4a3-188">Kopiert die Seite in einen bestimmten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="fd4a3-188">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
