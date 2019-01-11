---
title: notebook-Ressourcentyp
description: Stellt ein OneNote-Notizbuch dar.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: c39ac85dcfacb332a72c81d1d5f075a7a5021047
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876559"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="441d3-103">notebook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="441d3-103">notebook resource type</span></span>

> <span data-ttu-id="441d3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="441d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="441d3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="441d3-106">Stellt ein OneNote-Notizbuch dar.</span><span class="sxs-lookup"><span data-stu-id="441d3-106">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="441d3-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="441d3-107">JSON representation</span></span>

<span data-ttu-id="441d3-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="441d3-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a><span data-ttu-id="441d3-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="441d3-109">Properties</span></span>
| <span data-ttu-id="441d3-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="441d3-110">Property</span></span>     | <span data-ttu-id="441d3-111">Typ</span><span class="sxs-lookup"><span data-stu-id="441d3-111">Type</span></span>   |<span data-ttu-id="441d3-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="441d3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="441d3-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="441d3-113">createdBy</span></span>|[<span data-ttu-id="441d3-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="441d3-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="441d3-p102">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="441d3-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="441d3-117">createdDateTime</span></span>|<span data-ttu-id="441d3-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="441d3-118">DateTimeOffset</span></span>|<span data-ttu-id="441d3-p103">Das Datum und die Uhrzeit der Erstellung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-p103">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="441d3-123">id</span><span class="sxs-lookup"><span data-stu-id="441d3-123">id</span></span>|<span data-ttu-id="441d3-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="441d3-124">String</span></span>|<span data-ttu-id="441d3-p104">Der eindeutige Bezeichner des Notizbuchs. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-p104">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="441d3-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="441d3-127">isDefault</span></span>|<span data-ttu-id="441d3-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="441d3-128">Boolean</span></span>|<span data-ttu-id="441d3-p105">Gibt an, ob dies das Standardnotizbuch des Benutzers ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-p105">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="441d3-131">isShared</span><span class="sxs-lookup"><span data-stu-id="441d3-131">isShared</span></span>|<span data-ttu-id="441d3-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="441d3-132">Boolean</span></span>|<span data-ttu-id="441d3-p106">Gibt an, ob das Notizbuch freigegeben ist. Wenn „true“, können auch andere Personen als der Besitzer den Inhalt des Notizbuchs sehen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-p106">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="441d3-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="441d3-136">lastModifiedBy</span></span>|[<span data-ttu-id="441d3-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="441d3-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="441d3-p107">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="441d3-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="441d3-140">lastModifiedDateTime</span></span>|<span data-ttu-id="441d3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="441d3-141">DateTimeOffset</span></span>|<span data-ttu-id="441d3-p108">Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-p108">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="441d3-146">links</span><span class="sxs-lookup"><span data-stu-id="441d3-146">links</span></span>|[<span data-ttu-id="441d3-147">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="441d3-147">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="441d3-p109">Links zum Öffnen des Notizbuchs. Der Link `oneNoteClientURL` öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebURL` öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="441d3-p109">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="441d3-151">displayName</span><span class="sxs-lookup"><span data-stu-id="441d3-151">displayName</span></span>|<span data-ttu-id="441d3-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="441d3-152">String</span></span>|<span data-ttu-id="441d3-153">Der Name des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="441d3-153">The name of the notebook.</span></span>|
|<span data-ttu-id="441d3-154">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="441d3-154">sectionGroupsUrl</span></span>|<span data-ttu-id="441d3-155">String</span><span class="sxs-lookup"><span data-stu-id="441d3-155">String</span></span>|<span data-ttu-id="441d3-p110">Die URL für die Navigationseigenschaft `sectionGroups`, die alle Abschnittsgruppen im Notizbuch zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-p110">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="441d3-158">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="441d3-158">sectionsUrl</span></span>|<span data-ttu-id="441d3-159">String</span><span class="sxs-lookup"><span data-stu-id="441d3-159">String</span></span>|<span data-ttu-id="441d3-p111">Die URL für die Navigationseigenschaft `sections`, die alle Abschnitte im Notizbuch zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-p111">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="441d3-162">self</span><span class="sxs-lookup"><span data-stu-id="441d3-162">self</span></span>|<span data-ttu-id="441d3-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="441d3-163">String</span></span>|<span data-ttu-id="441d3-p112">Der Endpunkt, an dem Sie Details zum Notizbuch abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-p112">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="441d3-166">userRole</span><span class="sxs-lookup"><span data-stu-id="441d3-166">userRole</span></span>|<span data-ttu-id="441d3-167">String</span><span class="sxs-lookup"><span data-stu-id="441d3-167">String</span></span>|<span data-ttu-id="441d3-p113">Mögliche Werte: `Owner`, `Contributor`, `Reader`, `None`. „Owner“ stellt Zugriff auf Besitzerebene auf das Notizbuch dar. „Contributor“ stellt Lese-/Schreibzugriff auf das Notizbuch dar. „Reader“ stellt schreibgeschützten Zugriff auf das Notizbuch dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="441d3-p113">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="441d3-173">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="441d3-173">Relationships</span></span>
| <span data-ttu-id="441d3-174">Beziehung</span><span class="sxs-lookup"><span data-stu-id="441d3-174">Relationship</span></span> | <span data-ttu-id="441d3-175">Typ</span><span class="sxs-lookup"><span data-stu-id="441d3-175">Type</span></span>   |<span data-ttu-id="441d3-176">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="441d3-176">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="441d3-177">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="441d3-177">sectionGroups</span></span>|<span data-ttu-id="441d3-178">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="441d3-178">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="441d3-p114">Die Abschnittsgruppen im Notizbuch. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="441d3-p114">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="441d3-182">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="441d3-182">sections</span></span>|<span data-ttu-id="441d3-183">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="441d3-183">[Section](section.md) collection</span></span>|<span data-ttu-id="441d3-p115">Die Abschnitte im Notizbuch. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="441d3-p115">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="441d3-187">Methoden</span><span class="sxs-lookup"><span data-stu-id="441d3-187">Methods</span></span>

| <span data-ttu-id="441d3-188">Methode</span><span class="sxs-lookup"><span data-stu-id="441d3-188">Method</span></span>           | <span data-ttu-id="441d3-189">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="441d3-189">Return Type</span></span>    |<span data-ttu-id="441d3-190">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="441d3-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="441d3-191">Notizbuch abrufen</span><span class="sxs-lookup"><span data-stu-id="441d3-191">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="441d3-192">Notebook</span><span class="sxs-lookup"><span data-stu-id="441d3-192">Notebook</span></span>](notebook.md) |<span data-ttu-id="441d3-193">Dient zum Lesen der Eigenschaften und Beziehungen des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="441d3-193">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="441d3-194">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="441d3-194">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="441d3-195">[recentNotebook](recentnotebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="441d3-195">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="441d3-196">Dient zum Abrufen einer Sammlung der zuletzt geöffneten Notizbücher des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="441d3-196">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="441d3-197">Abschnittsgruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="441d3-197">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="441d3-198">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="441d3-198">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="441d3-199">Dient zum Erstellen einer Abschnittsgruppe durch Veröffentlichung in der SectionGroups-Sammlung im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="441d3-199">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="441d3-200">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="441d3-200">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="441d3-201">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="441d3-201">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="441d3-202">Dient zum Abrufen einer Sammlung von Abschnittsgruppen im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="441d3-202">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="441d3-203">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="441d3-203">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="441d3-204">Section</span><span class="sxs-lookup"><span data-stu-id="441d3-204">Section</span></span>](section.md)| <span data-ttu-id="441d3-205">Dient zum Erstellen eines Abschnitts durch Veröffentlichung in der Sections-Sammlung im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="441d3-205">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="441d3-206">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="441d3-206">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="441d3-207">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="441d3-207">[Section](section.md) collection</span></span>| <span data-ttu-id="441d3-208">Dient zum Abrufen einer Sammlung von Abschnitten im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="441d3-208">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="441d3-209">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="441d3-209">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="441d3-210">Keine</span><span class="sxs-lookup"><span data-stu-id="441d3-210">None</span></span> | <span data-ttu-id="441d3-211">Kopiert ein Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="441d3-211">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
