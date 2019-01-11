---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Laufwerk
localization_priority: Priority
ms.openlocfilehash: 20f19e8d03d947b13429c8763a2e7139705b834b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835470"
---
# <a name="drive-resource-type"></a><span data-ttu-id="9adee-102">Drive-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9adee-102">Drive resource type</span></span>

<span data-ttu-id="9adee-103">Die drive-Ressource ist das Objekt der obersten Ebene innerhalb des OneDrive eines Benutzers oder einer Dokumentbibliothek in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9adee-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="9adee-p101">OneDrive-Benutzern steht immer mindestens ein Laufwerk zur Verfügung, das Standardlaufwerk. Benutzern ohne OneDrive-Lizenz steht möglicherweise kein Standardlaufwerk zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="9adee-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9adee-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9adee-106">JSON representation</span></span>

<span data-ttu-id="9adee-107">Es folgt eine JSON-Darstellung einer Laufwerksressource.</span><span class="sxs-lookup"><span data-stu-id="9adee-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="9adee-108">Die **drive**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="9adee-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
    "sharepointIds",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

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
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="9adee-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9adee-109">Properties</span></span>

| <span data-ttu-id="9adee-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9adee-110">Property</span></span>             | <span data-ttu-id="9adee-111">Typ</span><span class="sxs-lookup"><span data-stu-id="9adee-111">Type</span></span>                          | <span data-ttu-id="9adee-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9adee-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9adee-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="9adee-113">createdBy</span></span>            | <span data-ttu-id="9adee-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9adee-114">[identitySet][]</span></span>               | <span data-ttu-id="9adee-p102">Die Identität des Benutzers, des Geräts oder der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="9adee-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9adee-117">createdDateTime</span></span>      | <span data-ttu-id="9adee-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9adee-118">dateTimeOffset</span></span>                | <span data-ttu-id="9adee-p103">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="9adee-121">description</span><span class="sxs-lookup"><span data-stu-id="9adee-121">description</span></span>          | <span data-ttu-id="9adee-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9adee-122">String</span></span>                        | <span data-ttu-id="9adee-123">Stellt eine für den Benutzer sichtbare Beschreibung des Laufwerks bereit.</span><span class="sxs-lookup"><span data-stu-id="9adee-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="9adee-124">Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="9adee-124">Read-write.</span></span>
| <span data-ttu-id="9adee-125">driveType</span><span class="sxs-lookup"><span data-stu-id="9adee-125">driveType</span></span>            | <span data-ttu-id="9adee-126">String</span><span class="sxs-lookup"><span data-stu-id="9adee-126">String</span></span>                        | <span data-ttu-id="9adee-p105">Beschreibt den Typ des Laufwerks, der durch diese Ressource dargestellt wird. Persönliche OneDrive-Laufwerke geben `personal` zurück. OneDrive for Business gibt `business` zurück. SharePoint-Dokumentbibliotheken geben `documentLibrary` zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="9adee-132">id</span><span class="sxs-lookup"><span data-stu-id="9adee-132">id</span></span>                   | <span data-ttu-id="9adee-133">String</span><span class="sxs-lookup"><span data-stu-id="9adee-133">String</span></span>                        | <span data-ttu-id="9adee-p106">Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="9adee-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9adee-136">lastModifiedBy</span></span>       | <span data-ttu-id="9adee-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9adee-137">[identitySet][]</span></span>               | <span data-ttu-id="9adee-p107">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="9adee-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9adee-140">lastModifiedDateTime</span></span> | <span data-ttu-id="9adee-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9adee-141">dateTimeOffset</span></span>                | <span data-ttu-id="9adee-p108">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="9adee-144">name</span><span class="sxs-lookup"><span data-stu-id="9adee-144">name</span></span>                 | <span data-ttu-id="9adee-145">string</span><span class="sxs-lookup"><span data-stu-id="9adee-145">string</span></span>                        | <span data-ttu-id="9adee-p109">Der Name des Elements. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="9adee-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="9adee-148">owner</span><span class="sxs-lookup"><span data-stu-id="9adee-148">owner</span></span>                | [<span data-ttu-id="9adee-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="9adee-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="9adee-p110">Optional.  Das Benutzerkonto, das das Laufwerk besitzt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="9adee-153">quota</span><span class="sxs-lookup"><span data-stu-id="9adee-153">quota</span></span>                | [<span data-ttu-id="9adee-154">quota</span><span class="sxs-lookup"><span data-stu-id="9adee-154">quota</span></span>](quota.md)             | <span data-ttu-id="9adee-p111">Optional.  Informationen zum Speicherkontingent des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="9adee-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="9adee-158">sharepointIds</span></span>        | <span data-ttu-id="9adee-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="9adee-159">[sharepointIds][]</span></span>             | <span data-ttu-id="9adee-p112">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="9adee-162">System-</span><span class="sxs-lookup"><span data-stu-id="9adee-162">system</span></span>               | <span data-ttu-id="9adee-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="9adee-163">[systemFacet][]</span></span>               | <span data-ttu-id="9adee-164">Falls vorhanden, gibt an, dass es sich um ein vom System verwaltetes Laufwerk handelt.</span><span class="sxs-lookup"><span data-stu-id="9adee-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="9adee-165">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-165">Read-only.</span></span>
| <span data-ttu-id="9adee-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="9adee-166">webUrl</span></span>               | <span data-ttu-id="9adee-167">String (URL)</span><span class="sxs-lookup"><span data-stu-id="9adee-167">string (url)</span></span>                  | <span data-ttu-id="9adee-p114">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="9adee-173">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9adee-173">Relationships</span></span>

| <span data-ttu-id="9adee-174">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9adee-174">Relationship</span></span> | <span data-ttu-id="9adee-175">Typ</span><span class="sxs-lookup"><span data-stu-id="9adee-175">Type</span></span>                                 | <span data-ttu-id="9adee-176">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9adee-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="9adee-177">Elemente</span><span class="sxs-lookup"><span data-stu-id="9adee-177">items</span></span>        | <span data-ttu-id="9adee-178">[DriveItem](driveitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9adee-178">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="9adee-p115">Alle im Laufwerk enthaltenen Elemente. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="9adee-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="9adee-182">root</span><span class="sxs-lookup"><span data-stu-id="9adee-182">root</span></span>         | [<span data-ttu-id="9adee-183">DriveItem</span><span class="sxs-lookup"><span data-stu-id="9adee-183">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="9adee-p116">Der Stammordner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="9adee-186">Sonderfall</span><span class="sxs-lookup"><span data-stu-id="9adee-186">special</span></span>      | <span data-ttu-id="9adee-187">[DriveItem](driveitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9adee-187">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="9adee-p117">Sammlung gemeinsamer Ordner, die  in OneDrive zur Verfügung stehen. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="9adee-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="9adee-191">Liste</span><span class="sxs-lookup"><span data-stu-id="9adee-191">list</span></span>         | [<span data-ttu-id="9adee-192">List</span><span class="sxs-lookup"><span data-stu-id="9adee-192">List</span></span>](list.md)                      | <span data-ttu-id="9adee-193">Für Laufwerke in SharePoint-Liste der zugrunde liegenden Dokumentbibliothek.</span><span class="sxs-lookup"><span data-stu-id="9adee-193">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="9adee-194">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9adee-194">Read-only.</span></span> <span data-ttu-id="9adee-195">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="9adee-195">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="9adee-196">Methoden</span><span class="sxs-lookup"><span data-stu-id="9adee-196">Methods</span></span>

|                        <span data-ttu-id="9adee-197">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="9adee-197">Common task</span></span>                         |         <span data-ttu-id="9adee-198">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="9adee-198">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="9adee-199">[Abrufen der Laufwerks-Metadaten eines anderen Laufwerks][drive-get]</span><span class="sxs-lookup"><span data-stu-id="9adee-199">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="9adee-200">[Abrufen des Stammordners des Standardlaufwerks des Benutzers][item-get]</span><span class="sxs-lookup"><span data-stu-id="9adee-200">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="9adee-201">[Auflisten der untergeordneten Elemente des Laufwerks][item-children]</span><span class="sxs-lookup"><span data-stu-id="9adee-201">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="9adee-202">[Auflisten der Änderungen für alle Elemente auf dem Laufwerk][item-changes]</span><span class="sxs-lookup"><span data-stu-id="9adee-202">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="9adee-203">[Suchen nach Elementen auf dem Laufwerk][item-search]</span><span class="sxs-lookup"><span data-stu-id="9adee-203">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="9adee-204">Abrufen spezieller Ordner</span><span class="sxs-lookup"><span data-stu-id="9adee-204">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="9adee-205">In der vorstehenden Tabelle verwenden die Beispiele `/drive`, andere Pfade sind jedoch ebenfalls gültig.</span><span class="sxs-lookup"><span data-stu-id="9adee-205">In the previous table, the examples use `/drive`, but other pathes are valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/drive.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
