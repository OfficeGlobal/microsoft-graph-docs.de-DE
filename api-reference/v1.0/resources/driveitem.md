---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
ms.openlocfilehash: d73b43b0ba1d98f496b4a1b2a606ec9f95298efa
ms.sourcegitcommit: ebac77d2ca32438e552831de0258fe5e86fa225a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2018
ms.locfileid: "26602384"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="7061d-102">Ressourcentyp „DriveItem“</span><span class="sxs-lookup"><span data-stu-id="7061d-102">DriveItem resource type</span></span>

<span data-ttu-id="7061d-p101">Die **driveItem**-Ressource stellt eine Datei, einen Ordner oder ein anderes auf einem Laufwerk gespeichertes Element dar. Alle Dateisystemobjekte in OneDrive und SharePoint werden als **driveItem**-Ressourcen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7061d-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="7061d-105">Es gibt zwei Hauptmethoden zum Adressieren einer **driveItem**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="7061d-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="7061d-106">Durch den eindeutigen **driveItem**-Bezeichner unter Verwendung von `drive/items/{item-id}`</span><span class="sxs-lookup"><span data-stu-id="7061d-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="7061d-107">Durch den Dateisystempfad unter Verwendung von `/drive/root:/path/to/file`</span><span class="sxs-lookup"><span data-stu-id="7061d-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="7061d-p102">**DriveItem**-Ressourcen verfügen über als Eigenschaften modellierte Facets, die Daten zu den driveItem-Identitäten und -Funktionen bereitstellen. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="7061d-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="7061d-110">Ordner haben ein [**„folder“-Facet**][-Ordner]</span><span class="sxs-lookup"><span data-stu-id="7061d-110">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="7061d-111">Dateien haben eine [**„file“-Facet**][-Datei].</span><span class="sxs-lookup"><span data-stu-id="7061d-111">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="7061d-112">Bilder haben zusätzlich zu ihrem „file“-Facet ein [**„image“Facet**][-Bild].</span><span class="sxs-lookup"><span data-stu-id="7061d-112">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="7061d-113">Mit einer Kamera aufgenommene Bilder (Fotos) haben ein [**„photo“-Facet**][-Foto], das die Elemente als Foto identifiziert und als Eigenschaften das Aufnahmedatum sowie das zur Aufnahme verwendete Gerät aufführt.</span><span class="sxs-lookup"><span data-stu-id="7061d-113">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="7061d-114">Elemente mit dem **folder**-Facet fungieren als Elementcontainer und besitzen daher einen `children`-Verweis auf eine Sammlung von **driveItems** im jeweiligen Ordner.</span><span class="sxs-lookup"><span data-stu-id="7061d-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7061d-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7061d-115">JSON representation</span></span>

<span data-ttu-id="7061d-116">Es folgt eine JSON-Darstellung einer **driveItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="7061d-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="7061d-117">Die **driveItem**-Ressource wird von [**baseItem**][baseItem] abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="7061d-117">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
       "baseType": "microsoft.graph.baseItem",
       "optionalProperties": ["cTag", "children", "folder", "file", "image", "audio", "video",
       "location", "deleted", "specialFolder", "photo", "thumbnails", "searchResult", "remoteItem",
       "shared", "content", "@microsoft.graph.conflictBehavior", "@microsoft.graph.downloadUrl", "@content.sourceUrl",
       "sharepointIds"],
       "keyProperty": "id", "openType": true } -->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "content": { "@odata.type": "Edm.Stream" },
  "cTag": "string (etag)",
  "deleted": { "@odata.type": "microsoft.graph.deleted"},
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
  "remoteItem": { "@odata.type": "microsoft.graph.remoteItem" },
  "root": { "@odata.type": "microsoft.graph.root" },
  "searchResult": { "@odata.type": "microsoft.graph.searchResult" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "string",

  /* relationships */
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "microsoft.graph.driveItemVersion"}],

  /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "eTag": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": {"@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "string",

  /* instance annotations */
  "@microsoft.graph.conflictBehavior": "string",
  "@microsoft.graph.downloadUrl": "url",
  "@microsoft.graph.sourceUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="7061d-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7061d-118">Properties</span></span>

| <span data-ttu-id="7061d-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7061d-119">Property</span></span>             | <span data-ttu-id="7061d-120">Typ</span><span class="sxs-lookup"><span data-stu-id="7061d-120">Type</span></span>               | <span data-ttu-id="7061d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7061d-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="7061d-122">audio</span><span class="sxs-lookup"><span data-stu-id="7061d-122">audio</span></span>                | <span data-ttu-id="7061d-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="7061d-123">[audio][]</span></span>          | <span data-ttu-id="7061d-p103">Audiometadaten, wenn das Element eine Audiodatei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="7061d-126">content</span><span class="sxs-lookup"><span data-stu-id="7061d-126">content</span></span>              | <span data-ttu-id="7061d-127">Stream</span><span class="sxs-lookup"><span data-stu-id="7061d-127">Stream</span></span>             | <span data-ttu-id="7061d-128">Der Inhaltsdatenstrom, wenn das Element eine Datei ist</span><span class="sxs-lookup"><span data-stu-id="7061d-128">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="7061d-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="7061d-129">createdBy</span></span>            | <span data-ttu-id="7061d-130">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7061d-130">[identitySet][]</span></span>    | <span data-ttu-id="7061d-p104">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="7061d-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7061d-133">createdDateTime</span></span>      | <span data-ttu-id="7061d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7061d-134">DateTimeOffset</span></span>     | <span data-ttu-id="7061d-p105">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="7061d-137">cTag</span><span class="sxs-lookup"><span data-stu-id="7061d-137">cTag</span></span>                 | <span data-ttu-id="7061d-138">String</span><span class="sxs-lookup"><span data-stu-id="7061d-138">String</span></span>             | <span data-ttu-id="7061d-p106">Ein ETag für den Inhalt des Elements. Dieses ETag wird nicht geändert, wenn nur die Metadaten geändert werden. **Hinweis:** Diese Eigenschaft wird nicht zurückgegeben, wenn das Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="7061d-143">gelöscht</span><span class="sxs-lookup"><span data-stu-id="7061d-143">deleted</span></span>              | <span data-ttu-id="7061d-144">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="7061d-144">[deleted][]</span></span>        | <span data-ttu-id="7061d-p107">Informationen zum „gelöscht“-Zustand des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="7061d-147">description</span><span class="sxs-lookup"><span data-stu-id="7061d-147">description</span></span>          | <span data-ttu-id="7061d-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7061d-148">String</span></span>             | <span data-ttu-id="7061d-p108">Stellt eine für den Benutzer sichtbare Beschreibung des Elements bereit. Lese-/Schreibzugriff. Nur auf OneDrive Personal</span><span class="sxs-lookup"><span data-stu-id="7061d-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="7061d-152">eTag</span><span class="sxs-lookup"><span data-stu-id="7061d-152">eTag</span></span>                 | <span data-ttu-id="7061d-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7061d-153">String</span></span>             | <span data-ttu-id="7061d-p109">ETag des gesamten Elements (Metadaten + Inhalt). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="7061d-156">file</span><span class="sxs-lookup"><span data-stu-id="7061d-156">file</span></span>                 | <span data-ttu-id="7061d-157">[file][]</span><span class="sxs-lookup"><span data-stu-id="7061d-157">[file][]</span></span>           | <span data-ttu-id="7061d-p110">Dateimetadaten, wenn das Element eine Datei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="7061d-160">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="7061d-160">fileSystemInfo</span></span>       | <span data-ttu-id="7061d-161">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="7061d-161">[fileSystemInfo][]</span></span> | <span data-ttu-id="7061d-p111">Informationen zum Dateisystem des Clients. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="7061d-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="7061d-164">folder</span><span class="sxs-lookup"><span data-stu-id="7061d-164">folder</span></span>               | <span data-ttu-id="7061d-165">[folder][]</span><span class="sxs-lookup"><span data-stu-id="7061d-165">[folder][]</span></span>         | <span data-ttu-id="7061d-p112">Ordnermetadaten, wenn das Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="7061d-168">id</span><span class="sxs-lookup"><span data-stu-id="7061d-168">id</span></span>                   | <span data-ttu-id="7061d-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7061d-169">String</span></span>             | <span data-ttu-id="7061d-p113">Der eindeutige Bezeichner des Elements im Laufwerk. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="7061d-172">Abbildung</span><span class="sxs-lookup"><span data-stu-id="7061d-172">image</span></span>                | <span data-ttu-id="7061d-173">[image][]</span><span class="sxs-lookup"><span data-stu-id="7061d-173">[image][]</span></span>          | <span data-ttu-id="7061d-p114">Bildmetadaten, wenn das Element ein Bild ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="7061d-176">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7061d-176">lastModifiedBy</span></span>       | <span data-ttu-id="7061d-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7061d-177">[identitySet][]</span></span>    | <span data-ttu-id="7061d-p115">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="7061d-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7061d-180">lastModifiedDateTime</span></span> | <span data-ttu-id="7061d-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7061d-181">DateTimeOffset</span></span>     | <span data-ttu-id="7061d-p116">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="7061d-184">location</span><span class="sxs-lookup"><span data-stu-id="7061d-184">location</span></span>             | <span data-ttu-id="7061d-185">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="7061d-185">[geoCoordinates][]</span></span> | <span data-ttu-id="7061d-p117">Standortmetadaten, sofern das Element Standortdaten aufweist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="7061d-188">name</span><span class="sxs-lookup"><span data-stu-id="7061d-188">name</span></span>                 | <span data-ttu-id="7061d-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7061d-189">String</span></span>             | <span data-ttu-id="7061d-p118">Der Name des Elements (Dateiname und Erweiterung). Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="7061d-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="7061d-192">package</span><span class="sxs-lookup"><span data-stu-id="7061d-192">package</span></span>              | <span data-ttu-id="7061d-193">[package][]</span><span class="sxs-lookup"><span data-stu-id="7061d-193">[package][]</span></span>        | <span data-ttu-id="7061d-p119">Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="7061d-197">parentReference</span><span class="sxs-lookup"><span data-stu-id="7061d-197">parentReference</span></span>      | <span data-ttu-id="7061d-198">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="7061d-198">[itemReference][]</span></span>  | <span data-ttu-id="7061d-p120">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="7061d-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="7061d-201">Foto</span><span class="sxs-lookup"><span data-stu-id="7061d-201">photo</span></span>                | <span data-ttu-id="7061d-202">[photo][]</span><span class="sxs-lookup"><span data-stu-id="7061d-202">[photo][]</span></span>          | <span data-ttu-id="7061d-p121">Fotometadaten, wenn das Element ein Foto ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="7061d-205">Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="7061d-205">publication</span></span>          | <span data-ttu-id="7061d-206">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="7061d-206">[publicationFacet][]</span></span> | <span data-ttu-id="7061d-207">Stellt Informationen über den veröffentlichten oder ausgecheckten Status eines Elements an Stellen bereit, die solche Aktionen unterstützen.</span><span class="sxs-lookup"><span data-stu-id="7061d-207">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="7061d-208">Diese Eigenschaft wird standardmäßig nicht zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7061d-208">This property is not returned by default.</span></span> <span data-ttu-id="7061d-209">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-209">Read-only.</span></span> |
| <span data-ttu-id="7061d-210">remoteItem</span><span class="sxs-lookup"><span data-stu-id="7061d-210">remoteItem</span></span>           | <span data-ttu-id="7061d-211">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="7061d-211">[remoteItem][]</span></span>     | <span data-ttu-id="7061d-p123">Daten zum Remoteelement, wenn das Element von einem anderen Laufwerk freigegeben ist als dem, auf das zugegriffen wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p123">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="7061d-214">root</span><span class="sxs-lookup"><span data-stu-id="7061d-214">root</span></span>                 | <span data-ttu-id="7061d-215">[root][]</span><span class="sxs-lookup"><span data-stu-id="7061d-215">[root][]</span></span>           | <span data-ttu-id="7061d-216">Wenn diese Eigenschaft nicht Null ist, bedeutet dies, dass es sich bei der driveItem-Ressource um die oberste driveItem-Ressource auf dem Laufwerk handelt.</span><span class="sxs-lookup"><span data-stu-id="7061d-216">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="7061d-217">searchResult</span><span class="sxs-lookup"><span data-stu-id="7061d-217">searchResult</span></span>         | <span data-ttu-id="7061d-218">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="7061d-218">[searchResult][]</span></span>   | <span data-ttu-id="7061d-p124">Suchmetadaten, wenn das Element aus einem Suchergebnis stammt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p124">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="7061d-221">shared</span><span class="sxs-lookup"><span data-stu-id="7061d-221">shared</span></span>               | <span data-ttu-id="7061d-222">[shared][]</span><span class="sxs-lookup"><span data-stu-id="7061d-222">[shared][]</span></span>         | <span data-ttu-id="7061d-p125">Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p125">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="7061d-225">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="7061d-225">sharepointIds</span></span>        | <span data-ttu-id="7061d-226">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="7061d-226">[sharepointIds][]</span></span>  | <span data-ttu-id="7061d-p126">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p126">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="7061d-229">size</span><span class="sxs-lookup"><span data-stu-id="7061d-229">size</span></span>                 | <span data-ttu-id="7061d-230">Int64</span><span class="sxs-lookup"><span data-stu-id="7061d-230">Int64</span></span>              | <span data-ttu-id="7061d-p127">Größe des Elements in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p127">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="7061d-233">specialFolder</span><span class="sxs-lookup"><span data-stu-id="7061d-233">specialFolder</span></span>        | <span data-ttu-id="7061d-234">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="7061d-234">[specialFolder][]</span></span>  | <span data-ttu-id="7061d-p128">Facet, das zurückgegeben wird, wenn das aktuelle Element auch als spezieller Ordner verfügbar ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p128">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="7061d-237">video</span><span class="sxs-lookup"><span data-stu-id="7061d-237">video</span></span>                | <span data-ttu-id="7061d-238">[video][]</span><span class="sxs-lookup"><span data-stu-id="7061d-238">[video][]</span></span>          | <span data-ttu-id="7061d-p129">Videometadaten, wenn das Element ein Video ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p129">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="7061d-241">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="7061d-241">webDavUrl</span></span>            | <span data-ttu-id="7061d-242">String</span><span class="sxs-lookup"><span data-stu-id="7061d-242">String</span></span>             | <span data-ttu-id="7061d-243">WebDAV-kompatible URL für das Element.</span><span class="sxs-lookup"><span data-stu-id="7061d-243">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="7061d-244">webUrl</span><span class="sxs-lookup"><span data-stu-id="7061d-244">webUrl</span></span>               | <span data-ttu-id="7061d-245">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7061d-245">String</span></span>             | <span data-ttu-id="7061d-p130">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p130">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="7061d-p131">**Hinweis:** Die Eigenschaften „eTag“ und „cTag“ arbeiten bei Containern (Ordnern) anders. Der Wert „cTag“ wird geändert, wenn Inhalte oder Metadaten eines Nachfolgers des Ordners geändert werden. Der Wert „eTag“ wird nur geändert, wenn die Eigenschaften des Ordners geändert werden. Ausnahme: Eigenschaften, die von Nachfolgern abgeleitet werden (wie **childCount** oder **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="7061d-p131">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="7061d-251">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7061d-251">Relationships</span></span>

| <span data-ttu-id="7061d-252">Beziehung</span><span class="sxs-lookup"><span data-stu-id="7061d-252">Relationship</span></span>       | <span data-ttu-id="7061d-253">Typ</span><span class="sxs-lookup"><span data-stu-id="7061d-253">Type</span></span>                        | <span data-ttu-id="7061d-254">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7061d-254">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="7061d-255">children</span><span class="sxs-lookup"><span data-stu-id="7061d-255">children</span></span>           | <span data-ttu-id="7061d-256">DriveItem-Auflistung</span><span class="sxs-lookup"><span data-stu-id="7061d-256">driveItem collection</span></span>        | <span data-ttu-id="7061d-p132">Sammlung von Elementobjekten der direkten untergeordneten Elemente eines Elements. Nur Elemente, die Ordner repräsentieren, haben untergeordnete Elemente. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="7061d-p132">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="7061d-261">createdByUser</span><span class="sxs-lookup"><span data-stu-id="7061d-261">createdByUser</span></span>      | <span data-ttu-id="7061d-262">[user][]</span><span class="sxs-lookup"><span data-stu-id="7061d-262">[user][]</span></span>                    | <span data-ttu-id="7061d-263">Der Name des Benutzers, der das Element erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="7061d-263">Identity of the user who created the item.</span></span> <span data-ttu-id="7061d-264">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-264">Read-only.</span></span>
| <span data-ttu-id="7061d-265">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="7061d-265">lastModifiedByUser</span></span> | <span data-ttu-id="7061d-266">[user][]</span><span class="sxs-lookup"><span data-stu-id="7061d-266">[user][]</span></span>                    | <span data-ttu-id="7061d-267">Der Name des Benutzers, der das Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="7061d-267">Identity of the user who last modified the item.</span></span> <span data-ttu-id="7061d-268">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-268">Read-only.</span></span>
| <span data-ttu-id="7061d-269">listItem</span><span class="sxs-lookup"><span data-stu-id="7061d-269">listItem</span></span>           | <span data-ttu-id="7061d-270">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="7061d-270">[listItem][]</span></span>                | <span data-ttu-id="7061d-271">Für Laufwerke in SharePoint, die zugeordneten Dokumentbibliothek-Listenelement.</span><span class="sxs-lookup"><span data-stu-id="7061d-271">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="7061d-272">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-272">Read-only.</span></span> <span data-ttu-id="7061d-273">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="7061d-273">Nullable.</span></span>
| <span data-ttu-id="7061d-274">permissions</span><span class="sxs-lookup"><span data-stu-id="7061d-274">permissions</span></span>        | <span data-ttu-id="7061d-275">[permission][] collection</span><span class="sxs-lookup"><span data-stu-id="7061d-275">[permission][] collection</span></span>   | <span data-ttu-id="7061d-p136">Der Satz von Berechtigungen für das Element. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="7061d-p136">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="7061d-279">thumbnails</span><span class="sxs-lookup"><span data-stu-id="7061d-279">thumbnails</span></span>         | <span data-ttu-id="7061d-280">[thumbnailSet][] collection</span><span class="sxs-lookup"><span data-stu-id="7061d-280">[thumbnailSet][] collection</span></span> | <span data-ttu-id="7061d-p137">Sammlung der dem Element zugeordneten [ThumbnailSet][]-Objekte. Weitere Informationen finden Sie im Artikel zum [Abrufen von Miniaturansichten][]. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="7061d-p137">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="7061d-285">Versionen</span><span class="sxs-lookup"><span data-stu-id="7061d-285">versions</span></span>           | <span data-ttu-id="7061d-286">[DriveItemVersion][] -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7061d-286">[driveItemVersion][] collection</span></span> | <span data-ttu-id="7061d-287">Die Liste der vorherigen Versionen des Elements.</span><span class="sxs-lookup"><span data-stu-id="7061d-287">The list of previous versions of the item.</span></span> <span data-ttu-id="7061d-288">Weitere Informationen finden Sie unter [Abrufen von früheren Versionen][].</span><span class="sxs-lookup"><span data-stu-id="7061d-288">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="7061d-289">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-289">Read-only.</span></span> <span data-ttu-id="7061d-290">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="7061d-290">Nullable.</span></span>
| <span data-ttu-id="7061d-291">Arbeitsmappe</span><span class="sxs-lookup"><span data-stu-id="7061d-291">workbook</span></span>           | <span data-ttu-id="7061d-292">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="7061d-292">[workbook][]</span></span>                | <span data-ttu-id="7061d-293">Für Dateien, die Excel-Kalkulationstabellen sind, greift auf die Arbeitsmappe API die Kalkulationstabelle Inhalt entwickelt.</span><span class="sxs-lookup"><span data-stu-id="7061d-293">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="7061d-294">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="7061d-294">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="7061d-295">Instanzenattribute</span><span class="sxs-lookup"><span data-stu-id="7061d-295">Instance Attributes</span></span>

<span data-ttu-id="7061d-p140">Instanzenattribute sind Eigenschaften mit speziellem Verhalten. Diese Eigenschaften sind temporär. Sie definieren entweder, wie sich der Dienst verhalten soll, oder geben kurzfristige Eigenschaftswerte an, beispielsweise URLs zum Elementdownload, die ablaufen.</span><span class="sxs-lookup"><span data-stu-id="7061d-p140">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="7061d-298">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="7061d-298">Property name</span></span>                     | <span data-ttu-id="7061d-299">Typ</span><span class="sxs-lookup"><span data-stu-id="7061d-299">Type</span></span>   | <span data-ttu-id="7061d-300">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7061d-300">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="7061d-301">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="7061d-301">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="7061d-302">string</span><span class="sxs-lookup"><span data-stu-id="7061d-302">string</span></span> | <span data-ttu-id="7061d-p141">Das Konfliktlösungsverhalten von Aktionen, die ein neues Element erstellen. Verwenden Sie die Werte *fail*, *replace* oder *rename*. Das Standardformat für PUT ist *replace*. Ein Element wird nie mit dieser Anmerkung zurückgegeben. Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="7061d-p141">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="7061d-308">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="7061d-308">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="7061d-309">string</span><span class="sxs-lookup"><span data-stu-id="7061d-309">string</span></span> | <span data-ttu-id="7061d-p142">Eine URL, über die die Inhalte der Datei heruntergeladen werden können. Eine Authentifizierung ist mit dieser URL nicht erforderlich. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7061d-p142">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="7061d-313">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="7061d-313">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="7061d-314">string</span><span class="sxs-lookup"><span data-stu-id="7061d-314">string</span></span> | <span data-ttu-id="7061d-p143">Bei Ausgabe einer PUT-Anforderung kann der Dienst mithilfe dieser Instanzanmerkung angewiesen werden, den Inhalt der URL herunterzuladen und als diese Datei zu speichern. Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="7061d-p143">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="7061d-p144">**Hinweis:** Der Wert „@microsoft.graph.downloadUrl“ ist eine kurzlebige URL und kann nicht zwischengespeichert werden. Die URL ist nur für kurze Zeit (1 Stunde) verfügbar, bevor sie ungültig wird.</span><span class="sxs-lookup"><span data-stu-id="7061d-p144">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached. The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>

## <a name="methods"></a><span data-ttu-id="7061d-319">Methoden</span><span class="sxs-lookup"><span data-stu-id="7061d-319">Methods</span></span>

| <span data-ttu-id="7061d-320">Methode</span><span class="sxs-lookup"><span data-stu-id="7061d-320">Method</span></span>                                                   | <span data-ttu-id="7061d-321">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="7061d-321">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="7061d-322">Element abrufen</span><span class="sxs-lookup"><span data-stu-id="7061d-322">Get item</span></span>](../api/driveitem_get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="7061d-323">Untergeordnete Objekte auflisten</span><span class="sxs-lookup"><span data-stu-id="7061d-323">List children</span></span>](../api/driveitem_list_children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="7061d-324">Versionen auflisten</span><span class="sxs-lookup"><span data-stu-id="7061d-324">List versions</span></span>](../api/driveitem_list_versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="7061d-325">Create item</span><span class="sxs-lookup"><span data-stu-id="7061d-325">Create item</span></span>](../api/driveitem_post_children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="7061d-326">Update item</span><span class="sxs-lookup"><span data-stu-id="7061d-326">Update item</span></span>](../api/driveitem_update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="7061d-327">Upload content</span><span class="sxs-lookup"><span data-stu-id="7061d-327">Upload content</span></span>](../api/driveitem_put_content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="7061d-328">Inhalte herunterladen</span><span class="sxs-lookup"><span data-stu-id="7061d-328">Download content</span></span>](../api/driveitem_get_content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="7061d-329">[Bestimmtes Dateiformat herunterladen][download-format]</span><span class="sxs-lookup"><span data-stu-id="7061d-329">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="7061d-330">Element löschen</span><span class="sxs-lookup"><span data-stu-id="7061d-330">Delete item</span></span>](../api/driveitem_delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="7061d-331">Move item</span><span class="sxs-lookup"><span data-stu-id="7061d-331">Move item</span></span>](../api/driveitem_move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="7061d-332">Copy item</span><span class="sxs-lookup"><span data-stu-id="7061d-332">Copy item</span></span>](../api/driveitem_copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="7061d-333">Search items</span><span class="sxs-lookup"><span data-stu-id="7061d-333">Search items</span></span>](../api/driveitem_search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="7061d-334">List changes in a drive</span><span class="sxs-lookup"><span data-stu-id="7061d-334">List changes in a drive</span></span>](../api/driveitem_delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="7061d-335">List thumbnails</span><span class="sxs-lookup"><span data-stu-id="7061d-335">List thumbnails</span></span>](../api/driveitem_list_thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="7061d-336">Freigabelink erstellen</span><span class="sxs-lookup"><span data-stu-id="7061d-336">Create sharing link</span></span>](../api/driveitem_createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="7061d-337">Berechtigungen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="7061d-337">Add permissions</span></span>](../api/driveitem_invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="7061d-338">Berechtigungen auflisten</span><span class="sxs-lookup"><span data-stu-id="7061d-338">List permissions</span></span>](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="7061d-339">Delete permission</span><span class="sxs-lookup"><span data-stu-id="7061d-339">Delete permission</span></span>](../api/permission_delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="7061d-340">[Preview-Element][item-preview]</span><span class="sxs-lookup"><span data-stu-id="7061d-340">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveItem_preview.md

## <a name="remarks"></a><span data-ttu-id="7061d-341">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="7061d-341">Remarks</span></span>

<span data-ttu-id="7061d-342">In OneDrive for Business- oder SharePoint-Dokumentbibliotheken wird die Eigenschaft **cTag** nicht zurückgegeben, wenn die **driveItem**-Ressource ein [Ordner][]-Facet hat.</span><span class="sxs-lookup"><span data-stu-id="7061d-342">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseItem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem_get_content_format.md
[driveItemVersion]: driveItemVersion.md
[file]: file.md
[fileSystemInfo]: fileSystemInfo.md
[folder]: folder.md
[Abrufen von früheren Versionen]: ../api/driveitem_list_versions.md
[getting previous versions]: ../api/driveitem_list_versions.md
[Abrufen von Miniaturansichten]: ../api/driveitem_list_thumbnails.md
[getting thumbnails]: ../api/driveitem_list_thumbnails.md
[identitySet]: identitySet.md
[image]: image.md
[itemReference]: itemReference.md
[geoCoordinates]: geoCoordinates.md
[listItem]: listItem.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteItem.md
[root]: root.md
[searchResult]: searchResult.md
[shared]: shared.md
[sharepointIds]: sharepointIds.md
[specialFolder]: specialFolder.md
[thumbnailSet]: thumbnailSet.md
[video]: video.md
[workbook]: workbook.md
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
