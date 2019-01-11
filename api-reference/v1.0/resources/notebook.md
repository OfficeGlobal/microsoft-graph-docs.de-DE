---
title: notebook-Ressourcentyp
description: Stellt ein OneNote-Notizbuch dar.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 0a657ea6d5837674a7881bc9ef6095af5529355a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894446"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="809c2-103">notebook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="809c2-103">notebook resource type</span></span>

<span data-ttu-id="809c2-104">Stellt ein OneNote-Notizbuch dar.</span><span class="sxs-lookup"><span data-stu-id="809c2-104">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="809c2-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="809c2-105">JSON representation</span></span>

<span data-ttu-id="809c2-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="809c2-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="809c2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="809c2-107">Properties</span></span>
| <span data-ttu-id="809c2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="809c2-108">Property</span></span>     | <span data-ttu-id="809c2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="809c2-109">Type</span></span>   |<span data-ttu-id="809c2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="809c2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="809c2-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="809c2-111">createdBy</span></span>|[<span data-ttu-id="809c2-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="809c2-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="809c2-p101">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="809c2-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="809c2-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="809c2-115">createdDateTime</span></span>|<span data-ttu-id="809c2-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="809c2-116">DateTimeOffset</span></span>|<span data-ttu-id="809c2-p102">Das Datum und die Uhrzeit der Erstellung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="809c2-p102">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="809c2-121">id</span><span class="sxs-lookup"><span data-stu-id="809c2-121">id</span></span>|<span data-ttu-id="809c2-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="809c2-122">String</span></span>|<span data-ttu-id="809c2-p103">Der eindeutige Bezeichner des Notizbuchs. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="809c2-p103">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="809c2-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="809c2-125">isDefault</span></span>|<span data-ttu-id="809c2-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="809c2-126">Boolean</span></span>|<span data-ttu-id="809c2-p104">Gibt an, ob dies das Standardnotizbuch des Benutzers ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="809c2-p104">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="809c2-129">isShared</span><span class="sxs-lookup"><span data-stu-id="809c2-129">isShared</span></span>|<span data-ttu-id="809c2-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="809c2-130">Boolean</span></span>|<span data-ttu-id="809c2-p105">Gibt an, ob das Notizbuch freigegeben ist. Wenn „true“, können auch andere Personen als der Besitzer den Inhalt des Notizbuchs sehen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="809c2-p105">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="809c2-134">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="809c2-134">lastModifiedBy</span></span>|[<span data-ttu-id="809c2-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="809c2-135">identitySet</span></span>](identityset.md)|<span data-ttu-id="809c2-p106">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="809c2-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="809c2-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="809c2-138">lastModifiedDateTime</span></span>|<span data-ttu-id="809c2-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="809c2-139">DateTimeOffset</span></span>|<span data-ttu-id="809c2-p107">Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="809c2-p107">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="809c2-144">links</span><span class="sxs-lookup"><span data-stu-id="809c2-144">links</span></span>|[<span data-ttu-id="809c2-145">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="809c2-145">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="809c2-p108">Links zum Öffnen des Notizbuchs. Der Link `oneNoteClientURL` öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebURL` öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="809c2-p108">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="809c2-149">displayName</span><span class="sxs-lookup"><span data-stu-id="809c2-149">displayName</span></span>|<span data-ttu-id="809c2-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="809c2-150">String</span></span>|<span data-ttu-id="809c2-151">Der Name des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="809c2-151">The name of the notebook.</span></span>|
|<span data-ttu-id="809c2-152">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="809c2-152">sectionGroupsUrl</span></span>|<span data-ttu-id="809c2-153">String</span><span class="sxs-lookup"><span data-stu-id="809c2-153">String</span></span>|<span data-ttu-id="809c2-p109">Die URL für die Navigationseigenschaft `sectionGroups`, die alle Abschnittsgruppen im Notizbuch zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="809c2-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="809c2-156">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="809c2-156">sectionsUrl</span></span>|<span data-ttu-id="809c2-157">String</span><span class="sxs-lookup"><span data-stu-id="809c2-157">String</span></span>|<span data-ttu-id="809c2-p110">Die URL für die Navigationseigenschaft `sections`, die alle Abschnitte im Notizbuch zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="809c2-p110">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="809c2-160">self</span><span class="sxs-lookup"><span data-stu-id="809c2-160">self</span></span>|<span data-ttu-id="809c2-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="809c2-161">String</span></span>|<span data-ttu-id="809c2-p111">Der Endpunkt, an dem Sie Details zum Notizbuch abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="809c2-p111">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="809c2-164">userRole</span><span class="sxs-lookup"><span data-stu-id="809c2-164">userRole</span></span>|<span data-ttu-id="809c2-165">onenoteUserRole</span><span class="sxs-lookup"><span data-stu-id="809c2-165">onenoteUserRole</span></span>|<span data-ttu-id="809c2-p112">Mögliche Werte: `Owner`, `Contributor`, `Reader`, `None`. „Owner“ stellt Zugriff auf Besitzerebene auf das Notizbuch dar. „Contributor“ stellt Lese-/Schreibzugriff auf das Notizbuch dar. „Reader“ stellt schreibgeschützten Zugriff auf das Notizbuch dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="809c2-p112">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="809c2-171">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="809c2-171">Relationships</span></span>
| <span data-ttu-id="809c2-172">Beziehung</span><span class="sxs-lookup"><span data-stu-id="809c2-172">Relationship</span></span> | <span data-ttu-id="809c2-173">Typ</span><span class="sxs-lookup"><span data-stu-id="809c2-173">Type</span></span>   |<span data-ttu-id="809c2-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="809c2-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="809c2-175">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="809c2-175">sectionGroups</span></span>|<span data-ttu-id="809c2-176">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="809c2-176">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="809c2-p113">Die Abschnittsgruppen im Notizbuch. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="809c2-p113">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="809c2-180">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="809c2-180">sections</span></span>|<span data-ttu-id="809c2-181">[OnenoteSection](section.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="809c2-181">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="809c2-p114">Die Abschnitte im Notizbuch. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="809c2-p114">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="809c2-185">Methoden</span><span class="sxs-lookup"><span data-stu-id="809c2-185">Methods</span></span>

| <span data-ttu-id="809c2-186">Methode</span><span class="sxs-lookup"><span data-stu-id="809c2-186">Method</span></span>           | <span data-ttu-id="809c2-187">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="809c2-187">Return Type</span></span>    |<span data-ttu-id="809c2-188">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="809c2-188">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="809c2-189">Notizbuch abrufen</span><span class="sxs-lookup"><span data-stu-id="809c2-189">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="809c2-190">Notebook</span><span class="sxs-lookup"><span data-stu-id="809c2-190">Notebook</span></span>](notebook.md) |<span data-ttu-id="809c2-191">Dient zum Lesen der Eigenschaften und Beziehungen des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="809c2-191">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="809c2-192">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="809c2-192">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="809c2-193">[recentNotebook](recentnotebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="809c2-193">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="809c2-194">Dient zum Abrufen einer Sammlung der zuletzt geöffneten Notizbücher des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="809c2-194">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="809c2-195">Abschnittsgruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="809c2-195">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="809c2-196">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="809c2-196">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="809c2-197">Dient zum Erstellen einer Abschnittsgruppe durch Veröffentlichung in der SectionGroups-Sammlung im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="809c2-197">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="809c2-198">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="809c2-198">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="809c2-199">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="809c2-199">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="809c2-200">Dient zum Abrufen einer Sammlung von Abschnittsgruppen im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="809c2-200">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="809c2-201">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="809c2-201">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="809c2-202">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="809c2-202">OnenoteSection</span></span>](section.md)| <span data-ttu-id="809c2-203">Dient zum Erstellen eines Abschnitts durch Veröffentlichung in der Sections-Sammlung im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="809c2-203">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="809c2-204">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="809c2-204">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="809c2-205">[OnenoteSection](section.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="809c2-205">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="809c2-206">Dient zum Abrufen einer Sammlung von Abschnitten im angegebenen Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="809c2-206">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="809c2-207">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="809c2-207">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="809c2-208">Keine</span><span class="sxs-lookup"><span data-stu-id="809c2-208">None</span></span> | <span data-ttu-id="809c2-209">Kopiert ein Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="809c2-209">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
