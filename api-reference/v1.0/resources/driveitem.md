---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
localization_priority: Priority
ms.openlocfilehash: 9de5de7f945177b1ab5c9f9107a32129f0f38c10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894558"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="a89b9-102">Ressourcentyp „DriveItem“</span><span class="sxs-lookup"><span data-stu-id="a89b9-102">DriveItem resource type</span></span>

<span data-ttu-id="a89b9-p101">Die **driveItem**-Ressource stellt eine Datei, einen Ordner oder ein anderes auf einem Laufwerk gespeichertes Element dar. Alle Dateisystemobjekte in OneDrive und SharePoint werden als **driveItem**-Ressourcen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="a89b9-105">Es gibt zwei Hauptmethoden zum Adressieren einer **driveItem**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="a89b9-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="a89b9-106">Durch den eindeutigen **driveItem**-Bezeichner unter Verwendung von `drive/items/{item-id}`</span><span class="sxs-lookup"><span data-stu-id="a89b9-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="a89b9-107">Durch den Dateisystempfad unter Verwendung von `/drive/root:/path/to/file`</span><span class="sxs-lookup"><span data-stu-id="a89b9-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="a89b9-p102">**DriveItem**-Ressourcen verfügen über als Eigenschaften modellierte Facets, die Daten zu den driveItem-Identitäten und -Funktionen bereitstellen. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="a89b9-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="a89b9-110">Ordner haben ein [**„folder“-Facet**][-Ordner]</span><span class="sxs-lookup"><span data-stu-id="a89b9-110">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="a89b9-111">Dateien haben eine [**„file“-Facet**][-Datei].</span><span class="sxs-lookup"><span data-stu-id="a89b9-111">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="a89b9-112">Bilder haben zusätzlich zu ihrem „file“-Facet ein [**„image“Facet**][-Bild].</span><span class="sxs-lookup"><span data-stu-id="a89b9-112">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="a89b9-113">Mit einer Kamera aufgenommene Bilder (Fotos) haben ein [**„photo“-Facet**][-Foto], das die Elemente als Foto identifiziert und als Eigenschaften das Aufnahmedatum sowie das zur Aufnahme verwendete Gerät aufführt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-113">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="a89b9-114">Elemente mit dem **folder**-Facet fungieren als Elementcontainer und besitzen daher einen `children`-Verweis auf eine Sammlung von **driveItems** im jeweiligen Ordner.</span><span class="sxs-lookup"><span data-stu-id="a89b9-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a89b9-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a89b9-115">JSON representation</span></span>

<span data-ttu-id="a89b9-116">Es folgt eine JSON-Darstellung einer **driveItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="a89b9-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="a89b9-117">Die **driveItem**-Ressource wird von [**baseItem**][baseItem] abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="a89b9-117">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a89b9-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a89b9-118">Properties</span></span>

| <span data-ttu-id="a89b9-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a89b9-119">Property</span></span>             | <span data-ttu-id="a89b9-120">Typ</span><span class="sxs-lookup"><span data-stu-id="a89b9-120">Type</span></span>               | <span data-ttu-id="a89b9-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a89b9-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="a89b9-122">audio</span><span class="sxs-lookup"><span data-stu-id="a89b9-122">audio</span></span>                | <span data-ttu-id="a89b9-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-123">[audio][]</span></span>          | <span data-ttu-id="a89b9-p103">Audiometadaten, wenn das Element eine Audiodatei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="a89b9-126">content</span><span class="sxs-lookup"><span data-stu-id="a89b9-126">content</span></span>              | <span data-ttu-id="a89b9-127">Stream</span><span class="sxs-lookup"><span data-stu-id="a89b9-127">Stream</span></span>             | <span data-ttu-id="a89b9-128">Der Inhaltsdatenstrom, wenn das Element eine Datei ist</span><span class="sxs-lookup"><span data-stu-id="a89b9-128">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="a89b9-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="a89b9-129">createdBy</span></span>            | <span data-ttu-id="a89b9-130">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-130">[identitySet][]</span></span>    | <span data-ttu-id="a89b9-p104">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="a89b9-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a89b9-133">createdDateTime</span></span>      | <span data-ttu-id="a89b9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a89b9-134">DateTimeOffset</span></span>     | <span data-ttu-id="a89b9-p105">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="a89b9-137">cTag</span><span class="sxs-lookup"><span data-stu-id="a89b9-137">cTag</span></span>                 | <span data-ttu-id="a89b9-138">String</span><span class="sxs-lookup"><span data-stu-id="a89b9-138">String</span></span>             | <span data-ttu-id="a89b9-p106">Ein ETag für den Inhalt des Elements. Dieses ETag wird nicht geändert, wenn nur die Metadaten geändert werden. **Hinweis:** Diese Eigenschaft wird nicht zurückgegeben, wenn das Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="a89b9-143">gelöscht</span><span class="sxs-lookup"><span data-stu-id="a89b9-143">deleted</span></span>              | <span data-ttu-id="a89b9-144">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-144">[deleted][]</span></span>        | <span data-ttu-id="a89b9-p107">Informationen zum „gelöscht“-Zustand des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="a89b9-147">description</span><span class="sxs-lookup"><span data-stu-id="a89b9-147">description</span></span>          | <span data-ttu-id="a89b9-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a89b9-148">String</span></span>             | <span data-ttu-id="a89b9-p108">Stellt eine für den Benutzer sichtbare Beschreibung des Elements bereit. Lese-/Schreibzugriff. Nur auf OneDrive Personal</span><span class="sxs-lookup"><span data-stu-id="a89b9-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="a89b9-152">eTag</span><span class="sxs-lookup"><span data-stu-id="a89b9-152">eTag</span></span>                 | <span data-ttu-id="a89b9-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a89b9-153">String</span></span>             | <span data-ttu-id="a89b9-p109">ETag des gesamten Elements (Metadaten + Inhalt). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="a89b9-156">file</span><span class="sxs-lookup"><span data-stu-id="a89b9-156">file</span></span>                 | <span data-ttu-id="a89b9-157">[file][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-157">[file][]</span></span>           | <span data-ttu-id="a89b9-p110">Dateimetadaten, wenn das Element eine Datei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="a89b9-160">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="a89b9-160">fileSystemInfo</span></span>       | <span data-ttu-id="a89b9-161">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-161">[fileSystemInfo][]</span></span> | <span data-ttu-id="a89b9-p111">Informationen zum Dateisystem des Clients. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="a89b9-164">folder</span><span class="sxs-lookup"><span data-stu-id="a89b9-164">folder</span></span>               | <span data-ttu-id="a89b9-165">[folder][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-165">[folder][]</span></span>         | <span data-ttu-id="a89b9-p112">Ordnermetadaten, wenn das Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="a89b9-168">id</span><span class="sxs-lookup"><span data-stu-id="a89b9-168">id</span></span>                   | <span data-ttu-id="a89b9-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a89b9-169">String</span></span>             | <span data-ttu-id="a89b9-p113">Der eindeutige Bezeichner des Elements im Laufwerk. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="a89b9-172">Abbildung</span><span class="sxs-lookup"><span data-stu-id="a89b9-172">image</span></span>                | <span data-ttu-id="a89b9-173">[image][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-173">[image][]</span></span>          | <span data-ttu-id="a89b9-p114">Bildmetadaten, wenn das Element ein Bild ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="a89b9-176">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a89b9-176">lastModifiedBy</span></span>       | <span data-ttu-id="a89b9-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-177">[identitySet][]</span></span>    | <span data-ttu-id="a89b9-p115">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="a89b9-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a89b9-180">lastModifiedDateTime</span></span> | <span data-ttu-id="a89b9-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a89b9-181">DateTimeOffset</span></span>     | <span data-ttu-id="a89b9-p116">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="a89b9-184">location</span><span class="sxs-lookup"><span data-stu-id="a89b9-184">location</span></span>             | <span data-ttu-id="a89b9-185">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-185">[geoCoordinates][]</span></span> | <span data-ttu-id="a89b9-p117">Standortmetadaten, sofern das Element Standortdaten aufweist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="a89b9-188">name</span><span class="sxs-lookup"><span data-stu-id="a89b9-188">name</span></span>                 | <span data-ttu-id="a89b9-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a89b9-189">String</span></span>             | <span data-ttu-id="a89b9-p118">Der Name des Elements (Dateiname und Erweiterung). Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="a89b9-192">package</span><span class="sxs-lookup"><span data-stu-id="a89b9-192">package</span></span>              | <span data-ttu-id="a89b9-193">[package][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-193">[package][]</span></span>        | <span data-ttu-id="a89b9-p119">Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="a89b9-197">parentReference</span><span class="sxs-lookup"><span data-stu-id="a89b9-197">parentReference</span></span>      | <span data-ttu-id="a89b9-198">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-198">[itemReference][]</span></span>  | <span data-ttu-id="a89b9-p120">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="a89b9-201">Foto</span><span class="sxs-lookup"><span data-stu-id="a89b9-201">photo</span></span>                | <span data-ttu-id="a89b9-202">[photo][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-202">[photo][]</span></span>          | <span data-ttu-id="a89b9-p121">Fotometadaten, wenn das Element ein Foto ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="a89b9-205">Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="a89b9-205">publication</span></span>          | <span data-ttu-id="a89b9-206">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-206">[publicationFacet][]</span></span> | <span data-ttu-id="a89b9-207">Stellt Informationen über den veröffentlichten oder ausgecheckten Status eines Elements an Stellen bereit, die solche Aktionen unterstützen.</span><span class="sxs-lookup"><span data-stu-id="a89b9-207">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="a89b9-208">Diese Eigenschaft wird standardmäßig nicht zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a89b9-208">This property is not returned by default.</span></span> <span data-ttu-id="a89b9-209">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-209">Read-only.</span></span> |
| <span data-ttu-id="a89b9-210">remoteItem</span><span class="sxs-lookup"><span data-stu-id="a89b9-210">remoteItem</span></span>           | <span data-ttu-id="a89b9-211">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-211">[remoteItem][]</span></span>     | <span data-ttu-id="a89b9-p123">Daten zum Remoteelement, wenn das Element von einem anderen Laufwerk freigegeben ist als dem, auf das zugegriffen wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p123">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="a89b9-214">root</span><span class="sxs-lookup"><span data-stu-id="a89b9-214">root</span></span>                 | <span data-ttu-id="a89b9-215">[root][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-215">[root][]</span></span>           | <span data-ttu-id="a89b9-216">Wenn diese Eigenschaft nicht Null ist, bedeutet dies, dass es sich bei der driveItem-Ressource um die oberste driveItem-Ressource auf dem Laufwerk handelt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-216">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="a89b9-217">searchResult</span><span class="sxs-lookup"><span data-stu-id="a89b9-217">searchResult</span></span>         | <span data-ttu-id="a89b9-218">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-218">[searchResult][]</span></span>   | <span data-ttu-id="a89b9-p124">Suchmetadaten, wenn das Element aus einem Suchergebnis stammt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p124">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="a89b9-221">shared</span><span class="sxs-lookup"><span data-stu-id="a89b9-221">shared</span></span>               | <span data-ttu-id="a89b9-222">[shared][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-222">[shared][]</span></span>         | <span data-ttu-id="a89b9-p125">Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p125">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="a89b9-225">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="a89b9-225">sharepointIds</span></span>        | <span data-ttu-id="a89b9-226">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-226">[sharepointIds][]</span></span>  | <span data-ttu-id="a89b9-p126">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p126">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="a89b9-229">size</span><span class="sxs-lookup"><span data-stu-id="a89b9-229">size</span></span>                 | <span data-ttu-id="a89b9-230">Int64</span><span class="sxs-lookup"><span data-stu-id="a89b9-230">Int64</span></span>              | <span data-ttu-id="a89b9-p127">Größe des Elements in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p127">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="a89b9-233">specialFolder</span><span class="sxs-lookup"><span data-stu-id="a89b9-233">specialFolder</span></span>        | <span data-ttu-id="a89b9-234">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-234">[specialFolder][]</span></span>  | <span data-ttu-id="a89b9-p128">Facet, das zurückgegeben wird, wenn das aktuelle Element auch als spezieller Ordner verfügbar ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p128">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="a89b9-237">video</span><span class="sxs-lookup"><span data-stu-id="a89b9-237">video</span></span>                | <span data-ttu-id="a89b9-238">[video][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-238">[video][]</span></span>          | <span data-ttu-id="a89b9-p129">Videometadaten, wenn das Element ein Video ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p129">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="a89b9-241">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="a89b9-241">webDavUrl</span></span>            | <span data-ttu-id="a89b9-242">String</span><span class="sxs-lookup"><span data-stu-id="a89b9-242">String</span></span>             | <span data-ttu-id="a89b9-243">WebDAV-kompatible URL für das Element.</span><span class="sxs-lookup"><span data-stu-id="a89b9-243">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="a89b9-244">webUrl</span><span class="sxs-lookup"><span data-stu-id="a89b9-244">webUrl</span></span>               | <span data-ttu-id="a89b9-245">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a89b9-245">String</span></span>             | <span data-ttu-id="a89b9-p130">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p130">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="a89b9-p131">**Hinweis:** Die Eigenschaften „eTag“ und „cTag“ arbeiten bei Containern (Ordnern) anders. Der Wert „cTag“ wird geändert, wenn Inhalte oder Metadaten eines Nachfolgers des Ordners geändert werden. Der Wert „eTag“ wird nur geändert, wenn die Eigenschaften des Ordners geändert werden. Ausnahme: Eigenschaften, die von Nachfolgern abgeleitet werden (wie **childCount** oder **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="a89b9-p131">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="a89b9-251">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a89b9-251">Relationships</span></span>

| <span data-ttu-id="a89b9-252">Beziehung</span><span class="sxs-lookup"><span data-stu-id="a89b9-252">Relationship</span></span>       | <span data-ttu-id="a89b9-253">Typ</span><span class="sxs-lookup"><span data-stu-id="a89b9-253">Type</span></span>                        | <span data-ttu-id="a89b9-254">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a89b9-254">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="a89b9-255">children</span><span class="sxs-lookup"><span data-stu-id="a89b9-255">children</span></span>           | <span data-ttu-id="a89b9-256">DriveItem-Auflistung</span><span class="sxs-lookup"><span data-stu-id="a89b9-256">driveItem collection</span></span>        | <span data-ttu-id="a89b9-p132">Sammlung von Elementobjekten der direkten untergeordneten Elemente eines Elements. Nur Elemente, die Ordner repräsentieren, haben untergeordnete Elemente. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p132">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="a89b9-261">createdByUser</span><span class="sxs-lookup"><span data-stu-id="a89b9-261">createdByUser</span></span>      | <span data-ttu-id="a89b9-262">[user][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-262">[user][]</span></span>                    | <span data-ttu-id="a89b9-263">Der Name des Benutzers, der das Element erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="a89b9-263">Identity of the user who created the item.</span></span> <span data-ttu-id="a89b9-264">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-264">Read-only.</span></span>
| <span data-ttu-id="a89b9-265">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="a89b9-265">lastModifiedByUser</span></span> | <span data-ttu-id="a89b9-266">[user][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-266">[user][]</span></span>                    | <span data-ttu-id="a89b9-267">Der Name des Benutzers, der das Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="a89b9-267">Identity of the user who last modified the item.</span></span> <span data-ttu-id="a89b9-268">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-268">Read-only.</span></span>
| <span data-ttu-id="a89b9-269">listItem</span><span class="sxs-lookup"><span data-stu-id="a89b9-269">listItem</span></span>           | <span data-ttu-id="a89b9-270">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-270">[listItem][]</span></span>                | <span data-ttu-id="a89b9-271">Für Laufwerke in SharePoint, die zugeordneten Dokumentbibliothek-Listenelement.</span><span class="sxs-lookup"><span data-stu-id="a89b9-271">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="a89b9-272">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-272">Read-only.</span></span> <span data-ttu-id="a89b9-273">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a89b9-273">Nullable.</span></span>
| <span data-ttu-id="a89b9-274">permissions</span><span class="sxs-lookup"><span data-stu-id="a89b9-274">permissions</span></span>        | <span data-ttu-id="a89b9-275">[permission][] collection</span><span class="sxs-lookup"><span data-stu-id="a89b9-275">[permission][] collection</span></span>   | <span data-ttu-id="a89b9-p136">Der Satz von Berechtigungen für das Element. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p136">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="a89b9-279">thumbnails</span><span class="sxs-lookup"><span data-stu-id="a89b9-279">thumbnails</span></span>         | <span data-ttu-id="a89b9-280">[thumbnailSet][] collection</span><span class="sxs-lookup"><span data-stu-id="a89b9-280">[thumbnailSet][] collection</span></span> | <span data-ttu-id="a89b9-p137">Sammlung der dem Element zugeordneten [ThumbnailSet][]-Objekte. Weitere Informationen finden Sie im Artikel zum [Abrufen von Miniaturansichten][]. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p137">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="a89b9-285">Versionen</span><span class="sxs-lookup"><span data-stu-id="a89b9-285">versions</span></span>           | <span data-ttu-id="a89b9-286">[DriveItemVersion][] -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a89b9-286">[driveItemVersion][] collection</span></span> | <span data-ttu-id="a89b9-287">Die Liste der vorherigen Versionen des Elements.</span><span class="sxs-lookup"><span data-stu-id="a89b9-287">The list of previous versions of the item.</span></span> <span data-ttu-id="a89b9-288">Weitere Informationen finden Sie unter [Abrufen von früheren Versionen][].</span><span class="sxs-lookup"><span data-stu-id="a89b9-288">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="a89b9-289">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-289">Read-only.</span></span> <span data-ttu-id="a89b9-290">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a89b9-290">Nullable.</span></span>
| <span data-ttu-id="a89b9-291">Arbeitsmappe</span><span class="sxs-lookup"><span data-stu-id="a89b9-291">workbook</span></span>           | <span data-ttu-id="a89b9-292">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="a89b9-292">[workbook][]</span></span>                | <span data-ttu-id="a89b9-293">Für Dateien, die Excel-Kalkulationstabellen sind, greift auf die Arbeitsmappe API die Kalkulationstabelle Inhalt entwickelt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-293">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="a89b9-294">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a89b9-294">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="a89b9-295">Instanzenattribute</span><span class="sxs-lookup"><span data-stu-id="a89b9-295">Instance Attributes</span></span>

<span data-ttu-id="a89b9-p140">Instanzenattribute sind Eigenschaften mit speziellem Verhalten. Diese Eigenschaften sind temporär. Sie definieren entweder, wie sich der Dienst verhalten soll, oder geben kurzfristige Eigenschaftswerte an, beispielsweise URLs zum Elementdownload, die ablaufen.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p140">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="a89b9-298">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="a89b9-298">Property name</span></span>                     | <span data-ttu-id="a89b9-299">Typ</span><span class="sxs-lookup"><span data-stu-id="a89b9-299">Type</span></span>   | <span data-ttu-id="a89b9-300">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a89b9-300">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="a89b9-301">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="a89b9-301">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="a89b9-302">string</span><span class="sxs-lookup"><span data-stu-id="a89b9-302">string</span></span> | <span data-ttu-id="a89b9-p141">Das Konfliktlösungsverhalten von Aktionen, die ein neues Element erstellen. Verwenden Sie die Werte *fail*, *replace* oder *rename*. Das Standardformat für PUT ist *replace*. Ein Element wird nie mit dieser Anmerkung zurückgegeben. Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p141">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="a89b9-308">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="a89b9-308">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="a89b9-309">string</span><span class="sxs-lookup"><span data-stu-id="a89b9-309">string</span></span> | <span data-ttu-id="a89b9-p142">Eine URL, über die die Inhalte der Datei heruntergeladen werden können. Eine Authentifizierung ist mit dieser URL nicht erforderlich. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p142">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="a89b9-313">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="a89b9-313">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="a89b9-314">string</span><span class="sxs-lookup"><span data-stu-id="a89b9-314">string</span></span> | <span data-ttu-id="a89b9-p143">Bei Ausgabe einer PUT-Anforderung kann der Dienst mithilfe dieser Instanzanmerkung angewiesen werden, den Inhalt der URL herunterzuladen und als diese Datei zu speichern. Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p143">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="a89b9-p144">**Hinweis:** Der Wert „@microsoft.graph.downloadUrl“ ist eine kurzlebige URL und kann nicht zwischengespeichert werden. Die URL ist nur für kurze Zeit (1 Stunde) verfügbar, bevor sie ungültig wird.</span><span class="sxs-lookup"><span data-stu-id="a89b9-p144">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached. The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>

## <a name="methods"></a><span data-ttu-id="a89b9-319">Methoden</span><span class="sxs-lookup"><span data-stu-id="a89b9-319">Methods</span></span>

| <span data-ttu-id="a89b9-320">Methode</span><span class="sxs-lookup"><span data-stu-id="a89b9-320">Method</span></span>                                                   | <span data-ttu-id="a89b9-321">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="a89b9-321">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="a89b9-322">Element abrufen</span><span class="sxs-lookup"><span data-stu-id="a89b9-322">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="a89b9-323">Untergeordnete Objekte auflisten</span><span class="sxs-lookup"><span data-stu-id="a89b9-323">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="a89b9-324">Versionen auflisten</span><span class="sxs-lookup"><span data-stu-id="a89b9-324">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="a89b9-325">Create item</span><span class="sxs-lookup"><span data-stu-id="a89b9-325">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="a89b9-326">Update item</span><span class="sxs-lookup"><span data-stu-id="a89b9-326">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="a89b9-327">Upload content</span><span class="sxs-lookup"><span data-stu-id="a89b9-327">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="a89b9-328">Inhalte herunterladen</span><span class="sxs-lookup"><span data-stu-id="a89b9-328">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="a89b9-329">[Bestimmtes Dateiformat herunterladen][download-format]</span><span class="sxs-lookup"><span data-stu-id="a89b9-329">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="a89b9-330">Element löschen</span><span class="sxs-lookup"><span data-stu-id="a89b9-330">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="a89b9-331">Move item</span><span class="sxs-lookup"><span data-stu-id="a89b9-331">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="a89b9-332">Copy item</span><span class="sxs-lookup"><span data-stu-id="a89b9-332">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="a89b9-333">Search items</span><span class="sxs-lookup"><span data-stu-id="a89b9-333">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="a89b9-334">List changes in a drive</span><span class="sxs-lookup"><span data-stu-id="a89b9-334">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="a89b9-335">List thumbnails</span><span class="sxs-lookup"><span data-stu-id="a89b9-335">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="a89b9-336">Freigabelink erstellen</span><span class="sxs-lookup"><span data-stu-id="a89b9-336">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="a89b9-337">Berechtigungen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="a89b9-337">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="a89b9-338">Berechtigungen auflisten</span><span class="sxs-lookup"><span data-stu-id="a89b9-338">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="a89b9-339">Delete permission</span><span class="sxs-lookup"><span data-stu-id="a89b9-339">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="a89b9-340">[Preview-Element][item-preview]</span><span class="sxs-lookup"><span data-stu-id="a89b9-340">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md

## <a name="remarks"></a><span data-ttu-id="a89b9-341">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="a89b9-341">Remarks</span></span>

<span data-ttu-id="a89b9-342">In OneDrive for Business- oder SharePoint-Dokumentbibliotheken wird die Eigenschaft **cTag** nicht zurückgegeben, wenn die **driveItem**-Ressource ein [Ordner][]-Facet hat.</span><span class="sxs-lookup"><span data-stu-id="a89b9-342">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[Abrufen von früheren Versionen]: ../api/driveitem-list-versions.md
[getting previous versions]: ../api/driveitem-list-versions.md
[Abrufen von Miniaturansichten]: ../api/driveitem-list-thumbnails.md
[getting thumbnails]: ../api/driveitem-list-thumbnails.md
[identitySet]: identityset.md
[image]: image.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[listItem]: listitem.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteitem.md
[root]: root.md
[searchResult]: searchresult.md
[shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[thumbnailSet]: thumbnailset.md
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
