---
title: notebook-Ressourcentyp
description: Stellt ein OneNote-Notizbuch dar.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 96be6a41424260610794f9a0df4ef8e35dc1597f
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967333"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="5e613-103">notebook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5e613-103">notebook resource type</span></span>

<span data-ttu-id="5e613-104">Stellt ein OneNote-Notizbuch dar.</span><span class="sxs-lookup"><span data-stu-id="5e613-104">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e613-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5e613-105">JSON representation</span></span>

<span data-ttu-id="5e613-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5e613-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
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
## <a name="properties"></a><span data-ttu-id="5e613-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5e613-107">Properties</span></span>
| <span data-ttu-id="5e613-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5e613-108">Property</span></span>     | <span data-ttu-id="5e613-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5e613-109">Type</span></span>   |<span data-ttu-id="5e613-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e613-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e613-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="5e613-111">createdBy</span></span>|[<span data-ttu-id="5e613-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="5e613-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="5e613-p101">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e613-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="5e613-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e613-115">createdDateTime</span></span>|<span data-ttu-id="5e613-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e613-116">DateTimeOffset</span></span>|<span data-ttu-id="5e613-p102">Das Datum und die Uhrzeit der Erstellung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e613-p102">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="5e613-121">id</span><span class="sxs-lookup"><span data-stu-id="5e613-121">id</span></span>|<span data-ttu-id="5e613-122">string</span><span class="sxs-lookup"><span data-stu-id="5e613-122">String</span></span>|<span data-ttu-id="5e613-p103">Der eindeutige Bezeichner des Notizbuchs. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e613-p103">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="5e613-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="5e613-125">isDefault</span></span>|<span data-ttu-id="5e613-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e613-126">Boolean</span></span>|<span data-ttu-id="5e613-p104">Gibt an, ob dies das Standardnotizbuch des Benutzers ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e613-p104">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="5e613-129">isShared</span><span class="sxs-lookup"><span data-stu-id="5e613-129">isShared</span></span>|<span data-ttu-id="5e613-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e613-130">Boolean</span></span>|<span data-ttu-id="5e613-p105">Gibt an, ob das Notizbuch freigegeben ist. Wenn „true“, können auch andere Personen als der Besitzer den Inhalt des Notizbuchs sehen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e613-p105">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="5e613-134">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5e613-134">lastModifiedBy</span></span>|[<span data-ttu-id="5e613-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="5e613-135">identitySet</span></span>](identityset.md)|<span data-ttu-id="5e613-p106">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e613-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="5e613-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e613-138">lastModifiedDateTime</span></span>|<span data-ttu-id="5e613-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e613-139">DateTimeOffset</span></span>|<span data-ttu-id="5e613-p107">Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e613-p107">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="5e613-144">links</span><span class="sxs-lookup"><span data-stu-id="5e613-144">links</span></span>|[<span data-ttu-id="5e613-145">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="5e613-145">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="5e613-p108">Links zum Öffnen des Notizbuchs. Der Link `oneNoteClientURL` öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebURL` öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="5e613-p108">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="5e613-149">displayName</span><span class="sxs-lookup"><span data-stu-id="5e613-149">displayName</span></span>|<span data-ttu-id="5e613-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5e613-150">String</span></span>|<span data-ttu-id="5e613-151">Der Name des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="5e613-151">The name of the notebook.</span></span>|
|<span data-ttu-id="5e613-152">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="5e613-152">sectionGroupsUrl</span></span>|<span data-ttu-id="5e613-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5e613-153">String</span></span>|<span data-ttu-id="5e613-p109">Die URL für die Navigationseigenschaft `sectionGroups`, die alle Abschnittsgruppen im Notizbuch zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e613-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="5e613-156">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="5e613-156">sectionsUrl</span></span>|<span data-ttu-id="5e613-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5e613-157">String</span></span>|<span data-ttu-id="5e613-p110">Die URL für die Navigationseigenschaft `sections`, die alle Abschnitte im Notizbuch zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e613-p110">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="5e613-160">self</span><span class="sxs-lookup"><span data-stu-id="5e613-160">self</span></span>|<span data-ttu-id="5e613-161">String</span><span class="sxs-lookup"><span data-stu-id="5e613-161">String</span></span>|<span data-ttu-id="5e613-p111">Der Endpunkt, an dem Sie Details zum Notizbuch abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e613-p111">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="5e613-164">userRole</span><span class="sxs-lookup"><span data-stu-id="5e613-164">userRole</span></span>|<span data-ttu-id="5e613-165">onenoteUserRole</span><span class="sxs-lookup"><span data-stu-id="5e613-165">onenoteUserRole</span></span>|<span data-ttu-id="5e613-p112">Mögliche Werte: `Owner`, `Contributor`, `Reader`, `None`. „Owner“ stellt Zugriff auf Besitzerebene auf das Notizbuch dar. „Contributor“ stellt Lese-/Schreibzugriff auf das Notizbuch dar. „Reader“ stellt schreibgeschützten Zugriff auf das Notizbuch dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e613-p112">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e613-171">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5e613-171">Relationships</span></span>
| <span data-ttu-id="5e613-172">Beziehung</span><span class="sxs-lookup"><span data-stu-id="5e613-172">Relationship</span></span> | <span data-ttu-id="5e613-173">Typ</span><span class="sxs-lookup"><span data-stu-id="5e613-173">Type</span></span>   |<span data-ttu-id="5e613-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e613-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e613-175">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="5e613-175">sectionGroups</span></span>|<span data-ttu-id="5e613-176">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5e613-176">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="5e613-p113">Die Abschnittsgruppen im Notizbuch. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="5e613-p113">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="5e613-180">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="5e613-180">sections</span></span>|<span data-ttu-id="5e613-181">[OnenoteSection](section.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5e613-181">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="5e613-p114">Die Abschnitte im Notizbuch. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="5e613-p114">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="5e613-185">Methoden</span><span class="sxs-lookup"><span data-stu-id="5e613-185">Methods</span></span>

| <span data-ttu-id="5e613-186">Methode</span><span class="sxs-lookup"><span data-stu-id="5e613-186">Method</span></span>           | <span data-ttu-id="5e613-187">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5e613-187">Return Type</span></span>    |<span data-ttu-id="5e613-188">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e613-188">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e613-189">Notizbuch abrufen</span><span class="sxs-lookup"><span data-stu-id="5e613-189">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="5e613-190">Notebook</span><span class="sxs-lookup"><span data-stu-id="5e613-190">Notebook</span></span>](notebook.md) |<span data-ttu-id="5e613-191">Dient zum Lesen der Eigenschaften und Beziehungen des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="5e613-191">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="5e613-192">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="5e613-192">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="5e613-193">[recentNotebook](recentnotebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5e613-193">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="5e613-194">Dient zum Abrufen einer Sammlung der zuletzt geöffneten Notizbücher des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="5e613-194">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="5e613-195">getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="5e613-195">getNotebookFromWebUrl</span></span>](../api/notebook-getnotebookfromweburl.md) | [<span data-ttu-id="5e613-196">Notebook</span><span class="sxs-lookup"><span data-stu-id="5e613-196">Notebook</span></span>](notebook.md) | <span data-ttu-id="5e613-197">Abrufen der Eigenschaften und die Beziehungen eines Notebook-Objekts verwenden den URL-Pfad.</span><span class="sxs-lookup"><span data-stu-id="5e613-197">Retrieve the properties and relationships of a notebook object using its URL path.</span></span> |
|[<span data-ttu-id="5e613-198">Abschnittsgruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="5e613-198">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="5e613-199">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="5e613-199">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="5e613-200">Dient zum Erstellen einer Abschnittsgruppe durch Veröffentlichung in der SectionGroups-Sammlung im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="5e613-200">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="5e613-201">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="5e613-201">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="5e613-202">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5e613-202">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="5e613-203">Dient zum Abrufen einer Sammlung von Abschnittsgruppen im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="5e613-203">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="5e613-204">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="5e613-204">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="5e613-205">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="5e613-205">OnenoteSection</span></span>](section.md)| <span data-ttu-id="5e613-206">Dient zum Erstellen eines Abschnitts durch Veröffentlichung in der Sections-Sammlung im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="5e613-206">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="5e613-207">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="5e613-207">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="5e613-208">[OnenoteSection](section.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5e613-208">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="5e613-209">Dient zum Abrufen einer Sammlung von Abschnitten im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="5e613-209">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="5e613-210">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="5e613-210">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="5e613-211">Keine</span><span class="sxs-lookup"><span data-stu-id="5e613-211">None</span></span> | <span data-ttu-id="5e613-212">Kopiert ein Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="5e613-212">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
