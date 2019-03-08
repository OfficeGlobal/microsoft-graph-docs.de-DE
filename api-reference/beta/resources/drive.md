---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Laufwerk
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 82a14f6462604b732119b90d037b2fab711df5af
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480992"
---
# <a name="drive-resource-type"></a><span data-ttu-id="5ee74-102">Drive-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5ee74-102">drive resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ee74-103">Die drive-Ressource ist das Objekt der obersten Ebene innerhalb des OneDrive eines Benutzers oder einer Dokumentbibliothek in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5ee74-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="5ee74-p101">OneDrive-Benutzern steht immer mindestens ein Laufwerk zur Verfügung, das Standardlaufwerk. Benutzern ohne OneDrive-Lizenz steht möglicherweise kein Standardlaufwerk zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ee74-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5ee74-106">JSON representation</span></span>

<span data-ttu-id="5ee74-107">Es folgt eine JSON-Darstellung einer Laufwerksressource.</span><span class="sxs-lookup"><span data-stu-id="5ee74-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="5ee74-108">Die **drive**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="5ee74-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "activities",
    "createdBy",
    "createdDateTime",
    "description",
    "lastModifiedBy",
    "lastModifiedDateTime",
    "name",
    "webUrl",
    "items",
    "root",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="5ee74-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5ee74-109">Properties</span></span>

| <span data-ttu-id="5ee74-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5ee74-110">Property</span></span>             | <span data-ttu-id="5ee74-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5ee74-111">Type</span></span>                          | <span data-ttu-id="5ee74-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ee74-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5ee74-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="5ee74-113">createdBy</span></span>            | <span data-ttu-id="5ee74-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5ee74-114">[identitySet][]</span></span>               | <span data-ttu-id="5ee74-p102">Die Identität des Benutzers, des Geräts oder der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="5ee74-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee74-117">createdDateTime</span></span>      | <span data-ttu-id="5ee74-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee74-118">dateTimeOffset</span></span>                | <span data-ttu-id="5ee74-p103">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="5ee74-121">description</span><span class="sxs-lookup"><span data-stu-id="5ee74-121">description</span></span>          | <span data-ttu-id="5ee74-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5ee74-122">String</span></span>                        | <span data-ttu-id="5ee74-123">Stellt eine für den Benutzer sichtbare Beschreibung des Laufwerks bereit.</span><span class="sxs-lookup"><span data-stu-id="5ee74-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="5ee74-124">Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="5ee74-124">Read-write.</span></span>
| <span data-ttu-id="5ee74-125">driveType</span><span class="sxs-lookup"><span data-stu-id="5ee74-125">driveType</span></span>            | <span data-ttu-id="5ee74-126">String</span><span class="sxs-lookup"><span data-stu-id="5ee74-126">String</span></span>                        | <span data-ttu-id="5ee74-p105">Beschreibt den Typ des Laufwerks, der durch diese Ressource dargestellt wird. Persönliche OneDrive-Laufwerke geben `personal` zurück. OneDrive for Business gibt `business` zurück. SharePoint-Dokumentbibliotheken geben `documentLibrary` zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="5ee74-132">id</span><span class="sxs-lookup"><span data-stu-id="5ee74-132">id</span></span>                   | <span data-ttu-id="5ee74-133">String</span><span class="sxs-lookup"><span data-stu-id="5ee74-133">String</span></span>                        | <span data-ttu-id="5ee74-p106">Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="5ee74-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5ee74-136">lastModifiedBy</span></span>       | <span data-ttu-id="5ee74-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5ee74-137">[identitySet][]</span></span>               | <span data-ttu-id="5ee74-p107">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="5ee74-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee74-140">lastModifiedDateTime</span></span> | <span data-ttu-id="5ee74-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee74-141">dateTimeOffset</span></span>                | <span data-ttu-id="5ee74-p108">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="5ee74-144">name</span><span class="sxs-lookup"><span data-stu-id="5ee74-144">name</span></span>                 | <span data-ttu-id="5ee74-145">string</span><span class="sxs-lookup"><span data-stu-id="5ee74-145">string</span></span>                        | <span data-ttu-id="5ee74-p109">Der Name des Elements. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="5ee74-148">owner</span><span class="sxs-lookup"><span data-stu-id="5ee74-148">owner</span></span>                | [<span data-ttu-id="5ee74-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="5ee74-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="5ee74-p110">Optional.  Das Benutzerkonto, das das Laufwerk besitzt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="5ee74-153">quota</span><span class="sxs-lookup"><span data-stu-id="5ee74-153">quota</span></span>                | [<span data-ttu-id="5ee74-154">quota</span><span class="sxs-lookup"><span data-stu-id="5ee74-154">quota</span></span>](quota.md)             | <span data-ttu-id="5ee74-p111">Optional.  Informationen zum Speicherkontingent des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="5ee74-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="5ee74-158">sharepointIds</span></span>        | <span data-ttu-id="5ee74-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="5ee74-159">[sharepointIds][]</span></span>             | <span data-ttu-id="5ee74-p112">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="5ee74-162">System</span><span class="sxs-lookup"><span data-stu-id="5ee74-162">system</span></span>               | <span data-ttu-id="5ee74-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="5ee74-163">[systemFacet][]</span></span>               | <span data-ttu-id="5ee74-164">Falls vorhanden, gibt an, dass es sich um ein vom System verwaltetes Laufwerk handelt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="5ee74-165">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-165">Read-only.</span></span>
| <span data-ttu-id="5ee74-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="5ee74-166">webUrl</span></span>               | <span data-ttu-id="5ee74-167">String (URL)</span><span class="sxs-lookup"><span data-stu-id="5ee74-167">string (url)</span></span>                  | <span data-ttu-id="5ee74-p114">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="5ee74-173">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5ee74-173">Relationships</span></span>

| <span data-ttu-id="5ee74-174">Beziehung</span><span class="sxs-lookup"><span data-stu-id="5ee74-174">Relationship</span></span> | <span data-ttu-id="5ee74-175">Typ</span><span class="sxs-lookup"><span data-stu-id="5ee74-175">Type</span></span>                                 | <span data-ttu-id="5ee74-176">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ee74-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="5ee74-177">Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="5ee74-177">activities</span></span>   | <span data-ttu-id="5ee74-178">[itemActivity][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5ee74-178">[itemActivity][] collection</span></span>          | <span data-ttu-id="5ee74-179">Die Liste der letzten Aktivitäten, die für dieses Laufwerk durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="5ee74-179">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="5ee74-180">Elemente</span><span class="sxs-lookup"><span data-stu-id="5ee74-180">items</span></span>        | <span data-ttu-id="5ee74-181">[driveitem](driveitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="5ee74-181">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="5ee74-p115">Alle im Laufwerk enthaltenen Elemente. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="5ee74-185">root</span><span class="sxs-lookup"><span data-stu-id="5ee74-185">root</span></span>         | [<span data-ttu-id="5ee74-186">driveitem</span><span class="sxs-lookup"><span data-stu-id="5ee74-186">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="5ee74-p116">Der Stammordner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="5ee74-189">Sonderfall</span><span class="sxs-lookup"><span data-stu-id="5ee74-189">special</span></span>      | <span data-ttu-id="5ee74-190">[driveitem](driveitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="5ee74-190">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="5ee74-p117">Sammlung gemeinsamer Ordner, die  in OneDrive zur Verfügung stehen. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="5ee74-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="5ee74-194">following</span><span class="sxs-lookup"><span data-stu-id="5ee74-194">following</span></span>    | <span data-ttu-id="5ee74-195">[Driveitem](driveitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5ee74-195">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="5ee74-196">Die Liste von Elementen, denen der Benutzer folgt.</span><span class="sxs-lookup"><span data-stu-id="5ee74-196">The list of items the user is following.</span></span> <span data-ttu-id="5ee74-197">Nur in OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="5ee74-197">Only in OneDrive for Business.</span></span>

## <a name="methods"></a><span data-ttu-id="5ee74-198">Methoden</span><span class="sxs-lookup"><span data-stu-id="5ee74-198">Methods</span></span>

|                        <span data-ttu-id="5ee74-199">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="5ee74-199">Common task</span></span>                         |         <span data-ttu-id="5ee74-200">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="5ee74-200">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="5ee74-201">[Abrufen der Laufwerks-Metadaten eines anderen Laufwerks][drive-get]</span><span class="sxs-lookup"><span data-stu-id="5ee74-201">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="5ee74-202">[Abrufen des Stammordners des Standardlaufwerks des Benutzers][item-get]</span><span class="sxs-lookup"><span data-stu-id="5ee74-202">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="5ee74-203">[Auflisten der Aktivitäten unter dem Laufwerk][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="5ee74-203">[List activities under the Drive][drive-activities]</span></span>        | `GET /drive/activities`     |
| <span data-ttu-id="5ee74-204">[Auflisten der Elemente, denen gefolgt wird][drive-following]</span><span class="sxs-lookup"><span data-stu-id="5ee74-204">[List followed Items][drive-following]</span></span>                     | `GET /drive/following`      |
| <span data-ttu-id="5ee74-205">[Auflisten der untergeordneten Elemente des Laufwerks][item-children]</span><span class="sxs-lookup"><span data-stu-id="5ee74-205">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="5ee74-206">[Auflisten der Änderungen für alle Elemente auf dem Laufwerk][item-changes]</span><span class="sxs-lookup"><span data-stu-id="5ee74-206">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="5ee74-207">[Suchen nach Elementen auf dem Laufwerk][item-search]</span><span class="sxs-lookup"><span data-stu-id="5ee74-207">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="5ee74-208">Abrufen spezieller Ordner</span><span class="sxs-lookup"><span data-stu-id="5ee74-208">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="5ee74-209">In der vorstehenden Tabelle verwenden die Beispiele `/drive`, andere Pfade sind jedoch ebenfalls gültig.</span><span class="sxs-lookup"><span data-stu-id="5ee74-209">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

[itemActivity]: itemactivity.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-activities]: ../api/activities-list.md
[drive-following]: ../api/drive-list-following.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": {
    "Resources/Drive": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/drive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
