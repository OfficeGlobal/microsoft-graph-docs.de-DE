---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fa172301e633a6f001133d44cb3332a5e133efe2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516742"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="a4f8d-102">Ressourcentyp driveItem</span><span class="sxs-lookup"><span data-stu-id="a4f8d-102">driveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4f8d-p101">Die **driveItem**-Ressource stellt eine Datei, einen Ordner oder ein anderes auf einem Laufwerk gespeichertes Element dar. Alle Dateisystemobjekte in OneDrive und SharePoint werden als **driveItem**-Ressourcen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="a4f8d-105">Es gibt zwei Hauptmethoden zum Adressieren einer **driveItem**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="a4f8d-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="a4f8d-106">Durch den eindeutigen **driveItem**-Bezeichner unter Verwendung von `drive/items/{item-id}`</span><span class="sxs-lookup"><span data-stu-id="a4f8d-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="a4f8d-107">Durch den Dateisystempfad unter Verwendung von `/drive/root:/path/to/file`</span><span class="sxs-lookup"><span data-stu-id="a4f8d-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="a4f8d-p102">**DriveItem**-Ressourcen verfügen über als Eigenschaften modellierte Facets, die Daten zu den driveItem-Identitäten und -Funktionen bereitstellen. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="a4f8d-110">Ordner haben ein [**„folder“-Facet**][-Ordner]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-110">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="a4f8d-111">Dateien haben eine [**„file“-Facet**][-Datei].</span><span class="sxs-lookup"><span data-stu-id="a4f8d-111">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="a4f8d-112">Bilder haben zusätzlich zu ihrem „file“-Facet ein [**„image“Facet**][-Bild].</span><span class="sxs-lookup"><span data-stu-id="a4f8d-112">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="a4f8d-113">Mit einer Kamera aufgenommene Bilder (Fotos) haben ein [**„photo“-Facet**][-Foto], das die Elemente als Foto identifiziert und als Eigenschaften das Aufnahmedatum sowie das zur Aufnahme verwendete Gerät aufführt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-113">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="a4f8d-114">Elemente mit dem **folder**-Facet fungieren als Elementcontainer und besitzen daher einen `children`-Verweis auf eine Sammlung von **driveItems** im jeweiligen Ordner.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4f8d-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a4f8d-115">JSON representation</span></span>

<span data-ttu-id="a4f8d-116">Es folgt eine JSON-Darstellung einer **driveItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="a4f8d-117">Die **driveItem**-Ressource wird von [**baseItem**][baseItem] abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-117">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "content": { "@odata.type": "Edm.Stream" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "Collection(microsoft.graph.driveItemVersion)"}],

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

## <a name="properties"></a><span data-ttu-id="a4f8d-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a4f8d-118">Properties</span></span>

| <span data-ttu-id="a4f8d-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a4f8d-119">Property</span></span>             | <span data-ttu-id="a4f8d-120">Typ</span><span class="sxs-lookup"><span data-stu-id="a4f8d-120">Type</span></span>               | <span data-ttu-id="a4f8d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4f8d-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="a4f8d-122">audio</span><span class="sxs-lookup"><span data-stu-id="a4f8d-122">audio</span></span>                | <span data-ttu-id="a4f8d-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-123">[audio][]</span></span>          | <span data-ttu-id="a4f8d-p103">Audiometadaten, wenn das Element eine Audiodatei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="a4f8d-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="a4f8d-126">createdBy</span></span>            | <span data-ttu-id="a4f8d-127">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-127">[identitySet][]</span></span>    | <span data-ttu-id="a4f8d-p104">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="a4f8d-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4f8d-130">createdDateTime</span></span>      | <span data-ttu-id="a4f8d-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4f8d-131">DateTimeOffset</span></span>     | <span data-ttu-id="a4f8d-p105">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="a4f8d-134">cTag</span><span class="sxs-lookup"><span data-stu-id="a4f8d-134">cTag</span></span>                 | <span data-ttu-id="a4f8d-135">String</span><span class="sxs-lookup"><span data-stu-id="a4f8d-135">String</span></span>             | <span data-ttu-id="a4f8d-p106">Ein ETag für den Inhalt des Elements. Dieses ETag wird nicht geändert, wenn nur die Metadaten geändert werden. **Hinweis:** Diese Eigenschaft wird nicht zurückgegeben, wenn das Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="a4f8d-140">gelöscht</span><span class="sxs-lookup"><span data-stu-id="a4f8d-140">deleted</span></span>              | <span data-ttu-id="a4f8d-141">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-141">[deleted][]</span></span>        | <span data-ttu-id="a4f8d-p107">Informationen zum „gelöscht“-Zustand des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="a4f8d-144">description</span><span class="sxs-lookup"><span data-stu-id="a4f8d-144">description</span></span>          | <span data-ttu-id="a4f8d-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4f8d-145">String</span></span>             | <span data-ttu-id="a4f8d-p108">Stellt eine für den Benutzer sichtbare Beschreibung des Elements bereit. Lese-/Schreibzugriff. Nur auf OneDrive Personal</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="a4f8d-149">eTag</span><span class="sxs-lookup"><span data-stu-id="a4f8d-149">eTag</span></span>                 | <span data-ttu-id="a4f8d-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4f8d-150">String</span></span>             | <span data-ttu-id="a4f8d-p109">ETag des gesamten Elements (Metadaten + Inhalt). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="a4f8d-153">file</span><span class="sxs-lookup"><span data-stu-id="a4f8d-153">file</span></span>                 | <span data-ttu-id="a4f8d-154">[file][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-154">[file][]</span></span>           | <span data-ttu-id="a4f8d-p110">Dateimetadaten, wenn das Element eine Datei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="a4f8d-157">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="a4f8d-157">fileSystemInfo</span></span>       | <span data-ttu-id="a4f8d-158">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-158">[fileSystemInfo][]</span></span> | <span data-ttu-id="a4f8d-p111">Informationen zum Dateisystem des Clients. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="a4f8d-161">folder</span><span class="sxs-lookup"><span data-stu-id="a4f8d-161">folder</span></span>               | <span data-ttu-id="a4f8d-162">[Ordner][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-162">[folder][]</span></span>         | <span data-ttu-id="a4f8d-p112">Ordnermetadaten, wenn das Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="a4f8d-165">id</span><span class="sxs-lookup"><span data-stu-id="a4f8d-165">id</span></span>                   | <span data-ttu-id="a4f8d-166">string</span><span class="sxs-lookup"><span data-stu-id="a4f8d-166">String</span></span>             | <span data-ttu-id="a4f8d-p113">Der eindeutige Bezeichner des Elements im Laufwerk. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="a4f8d-169">Abbildung</span><span class="sxs-lookup"><span data-stu-id="a4f8d-169">image</span></span>                | <span data-ttu-id="a4f8d-170">[image][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-170">[image][]</span></span>          | <span data-ttu-id="a4f8d-p114">Bildmetadaten, wenn das Element ein Bild ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="a4f8d-173">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a4f8d-173">lastModifiedBy</span></span>       | <span data-ttu-id="a4f8d-174">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-174">[identitySet][]</span></span>    | <span data-ttu-id="a4f8d-p115">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="a4f8d-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4f8d-177">lastModifiedDateTime</span></span> | <span data-ttu-id="a4f8d-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4f8d-178">DateTimeOffset</span></span>     | <span data-ttu-id="a4f8d-p116">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="a4f8d-181">location</span><span class="sxs-lookup"><span data-stu-id="a4f8d-181">location</span></span>             | <span data-ttu-id="a4f8d-182">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-182">[geoCoordinates][]</span></span> | <span data-ttu-id="a4f8d-p117">Standortmetadaten, sofern das Element Standortdaten aufweist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="a4f8d-185">name</span><span class="sxs-lookup"><span data-stu-id="a4f8d-185">name</span></span>                 | <span data-ttu-id="a4f8d-186">String</span><span class="sxs-lookup"><span data-stu-id="a4f8d-186">String</span></span>             | <span data-ttu-id="a4f8d-p118">Der Name des Elements (Dateiname und Erweiterung). Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="a4f8d-189">package</span><span class="sxs-lookup"><span data-stu-id="a4f8d-189">package</span></span>              | <span data-ttu-id="a4f8d-190">[package][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-190">[package][]</span></span>        | <span data-ttu-id="a4f8d-p119">Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="a4f8d-194">parentReference</span><span class="sxs-lookup"><span data-stu-id="a4f8d-194">parentReference</span></span>      | <span data-ttu-id="a4f8d-195">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-195">[itemReference][]</span></span>  | <span data-ttu-id="a4f8d-p120">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="a4f8d-198">Foto</span><span class="sxs-lookup"><span data-stu-id="a4f8d-198">photo</span></span>                | <span data-ttu-id="a4f8d-199">[photo][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-199">[photo][]</span></span>          | <span data-ttu-id="a4f8d-p121">Fotometadaten, wenn das Element ein Foto ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="a4f8d-202">Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="a4f8d-202">publication</span></span>          | <span data-ttu-id="a4f8d-203">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-203">[publicationFacet][]</span></span> | <span data-ttu-id="a4f8d-204">Stellt Informationen über den veröffentlichten oder ausgecheckten Status eines Elements an Stellen bereit, die solche Aktionen unterstützen.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-204">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="a4f8d-205">Diese Eigenschaft wird standardmäßig nicht zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-205">This property is not returned by default.</span></span> <span data-ttu-id="a4f8d-206">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-206">Read-only.</span></span> |
| <span data-ttu-id="a4f8d-207">remoteItem</span><span class="sxs-lookup"><span data-stu-id="a4f8d-207">remoteItem</span></span>           | <span data-ttu-id="a4f8d-208">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-208">[remoteItem][]</span></span>     | <span data-ttu-id="a4f8d-p123">Daten zum Remoteelement, wenn das Element von einem anderen Laufwerk freigegeben ist als dem, auf das zugegriffen wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p123">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="a4f8d-211">root</span><span class="sxs-lookup"><span data-stu-id="a4f8d-211">root</span></span>                 | <span data-ttu-id="a4f8d-212">[root][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-212">[root][]</span></span>           | <span data-ttu-id="a4f8d-213">Wenn diese Eigenschaft nicht Null ist, bedeutet dies, dass es sich bei der driveItem-Ressource um die oberste driveItem-Ressource auf dem Laufwerk handelt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-213">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="a4f8d-214">searchResult</span><span class="sxs-lookup"><span data-stu-id="a4f8d-214">searchResult</span></span>         | <span data-ttu-id="a4f8d-215">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-215">[searchResult][]</span></span>   | <span data-ttu-id="a4f8d-p124">Suchmetadaten, wenn das Element aus einem Suchergebnis stammt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p124">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="a4f8d-218">freigegeben</span><span class="sxs-lookup"><span data-stu-id="a4f8d-218">shared</span></span>               | <span data-ttu-id="a4f8d-219">[shared][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-219">[shared][]</span></span>         | <span data-ttu-id="a4f8d-p125">Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p125">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="a4f8d-222">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="a4f8d-222">sharepointIds</span></span>        | <span data-ttu-id="a4f8d-223">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-223">[sharepointIds][]</span></span>  | <span data-ttu-id="a4f8d-p126">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p126">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="a4f8d-226">size</span><span class="sxs-lookup"><span data-stu-id="a4f8d-226">size</span></span>                 | <span data-ttu-id="a4f8d-227">Int64</span><span class="sxs-lookup"><span data-stu-id="a4f8d-227">Int64</span></span>              | <span data-ttu-id="a4f8d-p127">Größe des Elements in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p127">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="a4f8d-230">specialFolder</span><span class="sxs-lookup"><span data-stu-id="a4f8d-230">specialFolder</span></span>        | <span data-ttu-id="a4f8d-231">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-231">[specialFolder][]</span></span>  | <span data-ttu-id="a4f8d-p128">Facet, das zurückgegeben wird, wenn das aktuelle Element auch als spezieller Ordner verfügbar ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p128">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="a4f8d-234">video</span><span class="sxs-lookup"><span data-stu-id="a4f8d-234">video</span></span>                | <span data-ttu-id="a4f8d-235">[video][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-235">[video][]</span></span>          | <span data-ttu-id="a4f8d-p129">Videometadaten, wenn das Element ein Video ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p129">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="a4f8d-238">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="a4f8d-238">webDavUrl</span></span>            | <span data-ttu-id="a4f8d-239">String</span><span class="sxs-lookup"><span data-stu-id="a4f8d-239">String</span></span>             | <span data-ttu-id="a4f8d-240">WebDAV-kompatible URL für das Element.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-240">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="a4f8d-241">webUrl</span><span class="sxs-lookup"><span data-stu-id="a4f8d-241">webUrl</span></span>               | <span data-ttu-id="a4f8d-242">String</span><span class="sxs-lookup"><span data-stu-id="a4f8d-242">String</span></span>             | <span data-ttu-id="a4f8d-p130">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p130">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="a4f8d-p131">**Hinweis:** Die Eigenschaften „eTag“ und „cTag“ arbeiten bei Containern (Ordnern) anders. Der Wert „cTag“ wird geändert, wenn Inhalte oder Metadaten eines Nachfolgers des Ordners geändert werden. Der Wert „eTag“ wird nur geändert, wenn die Eigenschaften des Ordners geändert werden. Ausnahme: Eigenschaften, die von Nachfolgern abgeleitet werden (wie **childCount** oder **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p131">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="a4f8d-248">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a4f8d-248">Relationships</span></span>

| <span data-ttu-id="a4f8d-249">Beziehung</span><span class="sxs-lookup"><span data-stu-id="a4f8d-249">Relationship</span></span>       | <span data-ttu-id="a4f8d-250">Typ</span><span class="sxs-lookup"><span data-stu-id="a4f8d-250">Type</span></span>                            | <span data-ttu-id="a4f8d-251">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4f8d-251">Description</span></span>
|:-------------------|:--------------------------------|:--------------------------
| <span data-ttu-id="a4f8d-252">Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="a4f8d-252">activities</span></span>         | <span data-ttu-id="a4f8d-253">[ItemActivity][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a4f8d-253">[itemActivity][] collection</span></span>     | <span data-ttu-id="a4f8d-254">Die Liste der letzten Aktivitäten, die für dieses Element durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-254">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="a4f8d-255">analytics</span><span class="sxs-lookup"><span data-stu-id="a4f8d-255">analytics</span></span>          | <span data-ttu-id="a4f8d-256">[itemAnalytics][]-Ressource</span><span class="sxs-lookup"><span data-stu-id="a4f8d-256">[itemAnalytics][] resource</span></span>      | <span data-ttu-id="a4f8d-257">Analytics über die Aktivitäten anzeigen, die für dieses Element ausgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-257">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="a4f8d-258">content</span><span class="sxs-lookup"><span data-stu-id="a4f8d-258">content</span></span>            | <span data-ttu-id="a4f8d-259">Stream</span><span class="sxs-lookup"><span data-stu-id="a4f8d-259">Stream</span></span>                          | <span data-ttu-id="a4f8d-260">Der Inhaltsdatenstrom, wenn das Element eine Datei darstellt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-260">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="a4f8d-261">children</span><span class="sxs-lookup"><span data-stu-id="a4f8d-261">children</span></span>           | <span data-ttu-id="a4f8d-262">driveitem-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a4f8d-262">driveitem collection</span></span>            | <span data-ttu-id="a4f8d-p132">Sammlung von Elementobjekten der direkten untergeordneten Elemente eines Elements. Nur Elemente, die Ordner repräsentieren, haben untergeordnete Elemente. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p132">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="a4f8d-267">listItem</span><span class="sxs-lookup"><span data-stu-id="a4f8d-267">listItem</span></span>           | <span data-ttu-id="a4f8d-268">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-268">[listItem][]</span></span>                    | <span data-ttu-id="a4f8d-269">Für Laufwerke in SharePoint das zugehörige Dokumentbibliothek-Listenelement.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-269">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="a4f8d-270">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-270">Read-only.</span></span> <span data-ttu-id="a4f8d-271">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-271">Nullable.</span></span>
| <span data-ttu-id="a4f8d-272">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a4f8d-272">permissions</span></span>        | <span data-ttu-id="a4f8d-273">[permission][] collection</span><span class="sxs-lookup"><span data-stu-id="a4f8d-273">[permission][] collection</span></span>       | <span data-ttu-id="a4f8d-p134">Der Satz von Berechtigungen für das Element. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p134">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="a4f8d-277">thumbnails</span><span class="sxs-lookup"><span data-stu-id="a4f8d-277">thumbnails</span></span>         | <span data-ttu-id="a4f8d-278">[thumbnailSet][] collection</span><span class="sxs-lookup"><span data-stu-id="a4f8d-278">[thumbnailSet][] collection</span></span>     | <span data-ttu-id="a4f8d-p135">Sammlung der dem Element zugeordneten [ThumbnailSet][]-Objekte. Weitere Informationen finden Sie im Artikel zum [Abrufen von Miniaturansichten][]. Schreibgeschützt. Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p135">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="a4f8d-283">versions</span><span class="sxs-lookup"><span data-stu-id="a4f8d-283">versions</span></span>           | <span data-ttu-id="a4f8d-284">[driveItemVersion][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a4f8d-284">[driveItemVersion][] collection</span></span> | <span data-ttu-id="a4f8d-285">Die Liste der früheren Versionen des Elements.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-285">The list of previous versions of the item.</span></span> <span data-ttu-id="a4f8d-286">Weitere Informationen finden Sie unter [Abrufen früherer Versionen][].</span><span class="sxs-lookup"><span data-stu-id="a4f8d-286">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="a4f8d-287">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-287">Read-only.</span></span> <span data-ttu-id="a4f8d-288">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-288">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="a4f8d-289">Instanzenattribute</span><span class="sxs-lookup"><span data-stu-id="a4f8d-289">Instance Attributes</span></span>

<span data-ttu-id="a4f8d-p137">Instanzenattribute sind Eigenschaften mit speziellem Verhalten. Diese Eigenschaften sind temporär. Sie definieren entweder, wie sich der Dienst verhalten soll, oder geben kurzfristige Eigenschaftswerte an, beispielsweise URLs zum Elementdownload, die ablaufen.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p137">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="a4f8d-292">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="a4f8d-292">Property name</span></span>                     | <span data-ttu-id="a4f8d-293">Typ</span><span class="sxs-lookup"><span data-stu-id="a4f8d-293">Type</span></span>   | <span data-ttu-id="a4f8d-294">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4f8d-294">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="a4f8d-295">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="a4f8d-295">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="a4f8d-296">string</span><span class="sxs-lookup"><span data-stu-id="a4f8d-296">string</span></span> | <span data-ttu-id="a4f8d-p138">Das Konfliktlösungsverhalten von Aktionen, die ein neues Element erstellen. Verwenden Sie die Werte *fail*, *replace* oder *rename*. Das Standardformat für PUT ist *replace*. Ein Element wird nie mit dieser Anmerkung zurückgegeben. Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p138">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="a4f8d-302">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="a4f8d-302">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="a4f8d-303">string</span><span class="sxs-lookup"><span data-stu-id="a4f8d-303">string</span></span> | <span data-ttu-id="a4f8d-p139">Eine URL, über die die Inhalte der Datei heruntergeladen werden können. Eine Authentifizierung ist mit dieser URL nicht erforderlich. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p139">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="a4f8d-307">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="a4f8d-307">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="a4f8d-308">string</span><span class="sxs-lookup"><span data-stu-id="a4f8d-308">string</span></span> | <span data-ttu-id="a4f8d-p140">Bei Ausgabe einer PUT-Anforderung kann der Dienst mithilfe dieser Instanzanmerkung angewiesen werden, den Inhalt der URL herunterzuladen und als diese Datei zu speichern. Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-p140">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="a4f8d-311">**Hinweis:** Der @microsoft.graph.downloadUrl-Wert ist eine kurzlebige URL und kann nicht zwischengespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-311">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="a4f8d-312">Die URL ist verfügbar für einen kurzen Zeitraum (1 Stunde), bevor es ungültig ist.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-312">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span> <span data-ttu-id="a4f8d-313">Entfernen von Berechtigungen für einen Benutzer möglicherweise die URL nicht sofort ungültig.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-313">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

## <a name="methods"></a><span data-ttu-id="a4f8d-314">Methoden</span><span class="sxs-lookup"><span data-stu-id="a4f8d-314">Methods</span></span>

| <span data-ttu-id="a4f8d-315">Methode</span><span class="sxs-lookup"><span data-stu-id="a4f8d-315">Method</span></span>                                                   | <span data-ttu-id="a4f8d-316">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="a4f8d-316">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="a4f8d-317">Element abrufen</span><span class="sxs-lookup"><span data-stu-id="a4f8d-317">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="a4f8d-318">Aktivitäten auflisten</span><span class="sxs-lookup"><span data-stu-id="a4f8d-318">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="a4f8d-319">[Analysen abrufen][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-319">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="a4f8d-320">[Aktivitäten nach Intervall abrufen][]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-320">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="a4f8d-321">Untergeordnete Elemente auflisten</span><span class="sxs-lookup"><span data-stu-id="a4f8d-321">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="a4f8d-322">Versionen auflisten</span><span class="sxs-lookup"><span data-stu-id="a4f8d-322">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="a4f8d-323">Element erstellen</span><span class="sxs-lookup"><span data-stu-id="a4f8d-323">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="a4f8d-324">Update item</span><span class="sxs-lookup"><span data-stu-id="a4f8d-324">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="a4f8d-325">Upload content</span><span class="sxs-lookup"><span data-stu-id="a4f8d-325">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="a4f8d-326">Inhalte herunterladen</span><span class="sxs-lookup"><span data-stu-id="a4f8d-326">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="a4f8d-327">[Bestimmtes Dateiformat herunterladen][download-format]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-327">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="a4f8d-328">Element löschen</span><span class="sxs-lookup"><span data-stu-id="a4f8d-328">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="a4f8d-329">Move item</span><span class="sxs-lookup"><span data-stu-id="a4f8d-329">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="a4f8d-330">Copy item</span><span class="sxs-lookup"><span data-stu-id="a4f8d-330">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="a4f8d-331">Search items</span><span class="sxs-lookup"><span data-stu-id="a4f8d-331">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="a4f8d-332">List changes in a drive</span><span class="sxs-lookup"><span data-stu-id="a4f8d-332">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="a4f8d-333">List thumbnails</span><span class="sxs-lookup"><span data-stu-id="a4f8d-333">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="a4f8d-334">Create sharing link</span><span class="sxs-lookup"><span data-stu-id="a4f8d-334">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="a4f8d-335">Add permissions</span><span class="sxs-lookup"><span data-stu-id="a4f8d-335">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="a4f8d-336">List permissions</span><span class="sxs-lookup"><span data-stu-id="a4f8d-336">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="a4f8d-337">Berechtigung löschen</span><span class="sxs-lookup"><span data-stu-id="a4f8d-337">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="a4f8d-338">[DDE-Kanal WebSocket abrufen][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-338">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="a4f8d-339">[Element in Vorschau anzeigen][item-preview]</span><span class="sxs-lookup"><span data-stu-id="a4f8d-339">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[Analysen abrufen]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Aktivitäten nach Intervall abrufen]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="a4f8d-342">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="a4f8d-342">Remarks</span></span>

<span data-ttu-id="a4f8d-343">In OneDrive for Business- oder SharePoint-Dokumentbibliotheken wird die Eigenschaft **cTag** nicht zurückgegeben, wenn die **driveItem**-Ressource ein [Ordner][]-Facet hat.</span><span class="sxs-lookup"><span data-stu-id="a4f8d-343">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[Abrufen früherer Versionen]: ../api/driveitem-list-versions.md
[getting previous versions]: ../api/driveitem-list-versions.md
[Abrufen von Miniaturansichten]: ../api/driveitem-list-thumbnails.md
[getting thumbnails]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/driveitem-subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[List activities]: ../api/activities-list.md
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
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": {
    "Resources/Item": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/driveitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
