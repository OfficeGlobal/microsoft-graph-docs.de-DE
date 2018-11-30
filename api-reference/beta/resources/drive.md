---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Laufwerk
ms.openlocfilehash: c9926d0245b63a8d4545c4864b396624b82bf57a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065879"
---
# <a name="drive-resource-type"></a><span data-ttu-id="299f7-102">Laufwerk Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="299f7-102">drive resource type</span></span>

> <span data-ttu-id="299f7-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="299f7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="299f7-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="299f7-105">Die drive-Ressource ist das Objekt der obersten Ebene innerhalb des OneDrive eines Benutzers oder einer Dokumentbibliothek in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="299f7-105">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="299f7-p102">OneDrive-Benutzern steht immer mindestens ein Laufwerk zur Verfügung, das Standardlaufwerk. Benutzern ohne OneDrive-Lizenz steht möglicherweise kein Standardlaufwerk zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="299f7-p102">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="299f7-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="299f7-108">JSON representation</span></span>

<span data-ttu-id="299f7-109">Es folgt eine JSON-Darstellung einer Laufwerksressource.</span><span class="sxs-lookup"><span data-stu-id="299f7-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="299f7-110">Die **drive**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="299f7-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="299f7-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="299f7-111">Properties</span></span>

| <span data-ttu-id="299f7-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="299f7-112">Property</span></span>             | <span data-ttu-id="299f7-113">Typ</span><span class="sxs-lookup"><span data-stu-id="299f7-113">Type</span></span>                          | <span data-ttu-id="299f7-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="299f7-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="299f7-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="299f7-115">createdBy</span></span>            | <span data-ttu-id="299f7-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="299f7-116">[identitySet][]</span></span>               | <span data-ttu-id="299f7-p103">Die Identität des Benutzers, des Geräts oder der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="299f7-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="299f7-119">createdDateTime</span></span>      | <span data-ttu-id="299f7-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="299f7-120">dateTimeOffset</span></span>                | <span data-ttu-id="299f7-p104">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="299f7-123">description</span><span class="sxs-lookup"><span data-stu-id="299f7-123">description</span></span>          | <span data-ttu-id="299f7-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="299f7-124">String</span></span>                        | <span data-ttu-id="299f7-125">Stellt eine für den Benutzer sichtbare Beschreibung des Laufwerks bereit.</span><span class="sxs-lookup"><span data-stu-id="299f7-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="299f7-126">Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="299f7-126">Read-write.</span></span>
| <span data-ttu-id="299f7-127">driveType</span><span class="sxs-lookup"><span data-stu-id="299f7-127">driveType</span></span>            | <span data-ttu-id="299f7-128">String</span><span class="sxs-lookup"><span data-stu-id="299f7-128">String</span></span>                        | <span data-ttu-id="299f7-p106">Beschreibt den Typ des Laufwerks, der durch diese Ressource dargestellt wird. Persönliche OneDrive-Laufwerke geben `personal` zurück. OneDrive for Business gibt `business` zurück. SharePoint-Dokumentbibliotheken geben `documentLibrary` zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-p106">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="299f7-134">id</span><span class="sxs-lookup"><span data-stu-id="299f7-134">id</span></span>                   | <span data-ttu-id="299f7-135">String</span><span class="sxs-lookup"><span data-stu-id="299f7-135">String</span></span>                        | <span data-ttu-id="299f7-p107">Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-p107">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="299f7-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="299f7-138">lastModifiedBy</span></span>       | <span data-ttu-id="299f7-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="299f7-139">[identitySet][]</span></span>               | <span data-ttu-id="299f7-p108">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="299f7-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="299f7-142">lastModifiedDateTime</span></span> | <span data-ttu-id="299f7-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="299f7-143">dateTimeOffset</span></span>                | <span data-ttu-id="299f7-p109">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="299f7-146">name</span><span class="sxs-lookup"><span data-stu-id="299f7-146">name</span></span>                 | <span data-ttu-id="299f7-147">string</span><span class="sxs-lookup"><span data-stu-id="299f7-147">string</span></span>                        | <span data-ttu-id="299f7-p110">Der Name des Elements. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="299f7-p110">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="299f7-150">owner</span><span class="sxs-lookup"><span data-stu-id="299f7-150">owner</span></span>                | [<span data-ttu-id="299f7-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="299f7-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="299f7-p111">Optional.  Das Benutzerkonto, das das Laufwerk besitzt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-p111">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="299f7-155">quota</span><span class="sxs-lookup"><span data-stu-id="299f7-155">quota</span></span>                | [<span data-ttu-id="299f7-156">quota</span><span class="sxs-lookup"><span data-stu-id="299f7-156">quota</span></span>](quota.md)             | <span data-ttu-id="299f7-p112">Optional.  Informationen zum Speicherkontingent des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-p112">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="299f7-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="299f7-160">sharepointIds</span></span>        | <span data-ttu-id="299f7-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="299f7-161">[sharepointIds][]</span></span>             | <span data-ttu-id="299f7-p113">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-p113">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="299f7-164">System-</span><span class="sxs-lookup"><span data-stu-id="299f7-164">system</span></span>               | <span data-ttu-id="299f7-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="299f7-165">[systemFacet][]</span></span>               | <span data-ttu-id="299f7-166">Falls vorhanden, gibt an, dass es sich um ein vom System verwaltetes Laufwerk handelt.</span><span class="sxs-lookup"><span data-stu-id="299f7-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="299f7-167">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-167">Read-only.</span></span>
| <span data-ttu-id="299f7-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="299f7-168">webUrl</span></span>               | <span data-ttu-id="299f7-169">String (URL)</span><span class="sxs-lookup"><span data-stu-id="299f7-169">string (url)</span></span>                  | <span data-ttu-id="299f7-p115">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-p115">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="299f7-175">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="299f7-175">Relationships</span></span>

| <span data-ttu-id="299f7-176">Beziehung</span><span class="sxs-lookup"><span data-stu-id="299f7-176">Relationship</span></span> | <span data-ttu-id="299f7-177">Typ</span><span class="sxs-lookup"><span data-stu-id="299f7-177">Type</span></span>                                 | <span data-ttu-id="299f7-178">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="299f7-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="299f7-179">Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="299f7-179">activities</span></span>   | <span data-ttu-id="299f7-180">[itemActivity][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="299f7-180">[itemActivity][] collection</span></span>          | <span data-ttu-id="299f7-181">Die Liste der letzten Aktivitäten, die für dieses Laufwerk durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="299f7-181">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="299f7-182">Elemente</span><span class="sxs-lookup"><span data-stu-id="299f7-182">items</span></span>        | <span data-ttu-id="299f7-183">[driveitem](driveitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="299f7-183">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="299f7-p116">Alle im Laufwerk enthaltenen Elemente. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="299f7-p116">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="299f7-187">root</span><span class="sxs-lookup"><span data-stu-id="299f7-187">root</span></span>         | [<span data-ttu-id="299f7-188">driveitem</span><span class="sxs-lookup"><span data-stu-id="299f7-188">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="299f7-p117">Der Stammordner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="299f7-p117">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="299f7-191">Sonderfall</span><span class="sxs-lookup"><span data-stu-id="299f7-191">special</span></span>      | <span data-ttu-id="299f7-192">[driveitem](driveitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="299f7-192">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="299f7-p118">Sammlung gemeinsamer Ordner, die  in OneDrive zur Verfügung stehen. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="299f7-p118">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="299f7-196">in der folgenden</span><span class="sxs-lookup"><span data-stu-id="299f7-196">following</span></span>    | <span data-ttu-id="299f7-197">[DriveItem](driveitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="299f7-197">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="299f7-198">Die Liste der Elemente, die der Benutzer folgt.</span><span class="sxs-lookup"><span data-stu-id="299f7-198">The list of items the user is following.</span></span> <span data-ttu-id="299f7-199">Nur in OneDrive für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="299f7-199">Only in OneDrive for Business.</span></span>

## <a name="methods"></a><span data-ttu-id="299f7-200">Methoden</span><span class="sxs-lookup"><span data-stu-id="299f7-200">Methods</span></span>

|                        <span data-ttu-id="299f7-201">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="299f7-201">Common task</span></span>                         |         <span data-ttu-id="299f7-202">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="299f7-202">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="299f7-203">[Abrufen der Laufwerks-Metadaten eines anderen Laufwerks][drive-get]</span><span class="sxs-lookup"><span data-stu-id="299f7-203">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="299f7-204">[Abrufen des Stammordners des Standardlaufwerks des Benutzers][item-get]</span><span class="sxs-lookup"><span data-stu-id="299f7-204">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="299f7-205">[Auflisten der Aktivitäten unter dem Laufwerk][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="299f7-205">[List activities under the Drive][drive-activities]</span></span>        | `GET /drive/activities`     |
| <span data-ttu-id="299f7-206">[Liste gefolgt Elemente][drive-following]</span><span class="sxs-lookup"><span data-stu-id="299f7-206">[List followed Items][drive-following]</span></span>                     | `GET /drive/following`      |
| <span data-ttu-id="299f7-207">[Auflisten der untergeordneten Elemente des Laufwerks][item-children]</span><span class="sxs-lookup"><span data-stu-id="299f7-207">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="299f7-208">[Auflisten der Änderungen für alle Elemente auf dem Laufwerk][item-changes]</span><span class="sxs-lookup"><span data-stu-id="299f7-208">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="299f7-209">[Suchen nach Elementen auf dem Laufwerk][item-search]</span><span class="sxs-lookup"><span data-stu-id="299f7-209">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="299f7-210">Abrufen spezieller Ordner</span><span class="sxs-lookup"><span data-stu-id="299f7-210">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="299f7-211">Verwenden Sie in der vorherigen Tabelle, in den Beispielen `/drive`, aber andere Pfade sind ungültig.</span><span class="sxs-lookup"><span data-stu-id="299f7-211">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->