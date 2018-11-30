---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Laufwerk
ms.openlocfilehash: 0b178967f7eb8da8bdf8584bb13a7d4f9950392b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="drive-resource-type"></a><span data-ttu-id="04724-102">Drive-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="04724-102">Drive resource type</span></span>

<span data-ttu-id="04724-103">Die drive-Ressource ist das Objekt der obersten Ebene innerhalb des OneDrive eines Benutzers oder einer Dokumentbibliothek in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="04724-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="04724-p101">OneDrive-Benutzern steht immer mindestens ein Laufwerk zur Verfügung, das Standardlaufwerk. Benutzern ohne OneDrive-Lizenz steht möglicherweise kein Standardlaufwerk zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="04724-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04724-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="04724-106">JSON representation</span></span>

<span data-ttu-id="04724-107">Es folgt eine JSON-Darstellung einer Laufwerksressource.</span><span class="sxs-lookup"><span data-stu-id="04724-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="04724-108">Die **drive**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="04724-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.drive",
       "keyProperty": "id", 
       "optionalProperties": [ "activities", "createdBy", "createdDateTime", "description", "lastModifiedBy", "lastModifiedDateTime", "name", "webUrl", "items", "root", "special", "system"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
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

## <a name="properties"></a><span data-ttu-id="04724-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="04724-109">Properties</span></span>

| <span data-ttu-id="04724-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04724-110">Property</span></span>             | <span data-ttu-id="04724-111">Typ</span><span class="sxs-lookup"><span data-stu-id="04724-111">Type</span></span>                          | <span data-ttu-id="04724-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04724-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="04724-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="04724-113">createdBy</span></span>            | <span data-ttu-id="04724-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="04724-114">[identitySet][]</span></span>               | <span data-ttu-id="04724-p102">Die Identität des Benutzers, des Geräts oder der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="04724-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04724-117">createdDateTime</span></span>      | <span data-ttu-id="04724-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04724-118">dateTimeOffset</span></span>                | <span data-ttu-id="04724-p103">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="04724-121">description</span><span class="sxs-lookup"><span data-stu-id="04724-121">description</span></span>          | <span data-ttu-id="04724-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04724-122">String</span></span>                        | <span data-ttu-id="04724-123">Stellt eine für den Benutzer sichtbare Beschreibung des Laufwerks bereit.</span><span class="sxs-lookup"><span data-stu-id="04724-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="04724-124">Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="04724-124">Read-write.</span></span>
| <span data-ttu-id="04724-125">driveType</span><span class="sxs-lookup"><span data-stu-id="04724-125">driveType</span></span>            | <span data-ttu-id="04724-126">String</span><span class="sxs-lookup"><span data-stu-id="04724-126">String</span></span>                        | <span data-ttu-id="04724-p105">Beschreibt den Typ des Laufwerks, der durch diese Ressource dargestellt wird. Persönliche OneDrive-Laufwerke geben `personal` zurück. OneDrive for Business gibt `business` zurück. SharePoint-Dokumentbibliotheken geben `documentLibrary` zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="04724-132">id</span><span class="sxs-lookup"><span data-stu-id="04724-132">id</span></span>                   | <span data-ttu-id="04724-133">String</span><span class="sxs-lookup"><span data-stu-id="04724-133">String</span></span>                        | <span data-ttu-id="04724-p106">Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="04724-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="04724-136">lastModifiedBy</span></span>       | <span data-ttu-id="04724-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="04724-137">[identitySet][]</span></span>               | <span data-ttu-id="04724-p107">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="04724-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04724-140">lastModifiedDateTime</span></span> | <span data-ttu-id="04724-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04724-141">dateTimeOffset</span></span>                | <span data-ttu-id="04724-p108">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="04724-144">name</span><span class="sxs-lookup"><span data-stu-id="04724-144">name</span></span>                 | <span data-ttu-id="04724-145">string</span><span class="sxs-lookup"><span data-stu-id="04724-145">string</span></span>                        | <span data-ttu-id="04724-p109">Der Name des Elements. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="04724-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="04724-148">owner</span><span class="sxs-lookup"><span data-stu-id="04724-148">owner</span></span>                | [<span data-ttu-id="04724-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="04724-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="04724-p110">Optional.  Das Benutzerkonto, das das Laufwerk besitzt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="04724-153">quota</span><span class="sxs-lookup"><span data-stu-id="04724-153">quota</span></span>                | [<span data-ttu-id="04724-154">quota</span><span class="sxs-lookup"><span data-stu-id="04724-154">quota</span></span>](quota.md)             | <span data-ttu-id="04724-p111">Optional.  Informationen zum Speicherkontingent des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="04724-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="04724-158">sharepointIds</span></span>        | <span data-ttu-id="04724-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="04724-159">[sharepointIds][]</span></span>             | <span data-ttu-id="04724-p112">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="04724-162">System</span><span class="sxs-lookup"><span data-stu-id="04724-162">System</span></span>               | <span data-ttu-id="04724-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="04724-163">[systemFacet][]</span></span>               | <span data-ttu-id="04724-164">Falls vorhanden, gibt an, dass es sich um ein vom System verwaltetes Laufwerk handelt.</span><span class="sxs-lookup"><span data-stu-id="04724-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="04724-165">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-165">Read-only.</span></span>
| <span data-ttu-id="04724-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="04724-166">webUrl</span></span>               | <span data-ttu-id="04724-167">String (URL)</span><span class="sxs-lookup"><span data-stu-id="04724-167">string (url)</span></span>                  | <span data-ttu-id="04724-p114">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="04724-173">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="04724-173">Relationships</span></span>

| <span data-ttu-id="04724-174">Beziehung</span><span class="sxs-lookup"><span data-stu-id="04724-174">Relationship</span></span> | <span data-ttu-id="04724-175">Typ</span><span class="sxs-lookup"><span data-stu-id="04724-175">Type</span></span>                                 | <span data-ttu-id="04724-176">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04724-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="04724-177">items</span><span class="sxs-lookup"><span data-stu-id="04724-177">items</span></span>        | <span data-ttu-id="04724-178">[driveitem](driveitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="04724-178">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="04724-p115">Alle im Laufwerk enthaltenen Elemente. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="04724-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="04724-182">root</span><span class="sxs-lookup"><span data-stu-id="04724-182">root</span></span>         | [<span data-ttu-id="04724-183">driveitem</span><span class="sxs-lookup"><span data-stu-id="04724-183">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="04724-p116">Der Stammordner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="04724-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="04724-186">Sonderfall</span><span class="sxs-lookup"><span data-stu-id="04724-186">special</span></span>      | <span data-ttu-id="04724-187">[driveitem](driveitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="04724-187">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="04724-p117">Sammlung gemeinsamer Ordner, die  in OneDrive zur Verfügung stehen. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="04724-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="04724-191">Methoden</span><span class="sxs-lookup"><span data-stu-id="04724-191">Methods</span></span>

|                        <span data-ttu-id="04724-192">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="04724-192">Common task</span></span>                         |         <span data-ttu-id="04724-193">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="04724-193">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="04724-194">[Abrufen der Laufwerks-Metadaten eines anderen Laufwerks][drive-get]</span><span class="sxs-lookup"><span data-stu-id="04724-194">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="04724-195">[Abrufen des Stammordners des Standardlaufwerks des Benutzers][item-get]</span><span class="sxs-lookup"><span data-stu-id="04724-195">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="04724-196">[Auflisten der untergeordneten Elemente des Laufwerks][item-children]</span><span class="sxs-lookup"><span data-stu-id="04724-196">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="04724-197">[Auflisten der Änderungen für alle Elemente auf dem Laufwerk][item-changes]</span><span class="sxs-lookup"><span data-stu-id="04724-197">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="04724-198">[Suchen nach Elementen auf dem Laufwerk][item-search]</span><span class="sxs-lookup"><span data-stu-id="04724-198">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="04724-199">Abrufen spezieller Ordner</span><span class="sxs-lookup"><span data-stu-id="04724-199">Access special folder</span></span>](../api/drive_get_specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="04724-200">In der vorstehenden Tabelle verwenden die Beispiele `/drive`, andere Pfade sind jedoch ebenfalls gültig.</span><span class="sxs-lookup"><span data-stu-id="04724-200">In the previous table, the examples use , but  is valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive_get.md
[item-get]: ../api/driveitem_get.md
[item-changes]: ../api/driveitem_delta.md
[item-search]: ../api/driveitem_search.md
[item-children]: ../api/driveitem_list_children.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
