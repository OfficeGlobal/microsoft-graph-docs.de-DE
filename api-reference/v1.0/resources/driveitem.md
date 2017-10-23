---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
ms.openlocfilehash: 526001ad9a6c52c5b031c1734466772861f1c67e
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="f642c-102">DriveItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f642c-102">DriveItem resource type</span></span>

<span data-ttu-id="f642c-p101">Die **driveItem**-Ressource stellt eine Datei, einen Ordner oder ein anderes auf einem Laufwerk gespeichertes Element dar. Alle Dateisystemobjekte in OneDrive und SharePoint werden als **driveItem**-Ressourcen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f642c-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="f642c-105">Es gibt zwei Hauptmethoden zum Adressieren einer **driveItem**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="f642c-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="f642c-106">Durch den eindeutigen **driveItem**-Bezeichner unter Verwendung von `drive/items/{item-id}`</span><span class="sxs-lookup"><span data-stu-id="f642c-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="f642c-107">Durch den Dateisystempfad unter Verwendung von `/drive/root:/path/to/file`</span><span class="sxs-lookup"><span data-stu-id="f642c-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="f642c-p102">**DriveItem**-Ressourcen verfügen über als Eigenschaften modellierte Facets, die Daten zu den driveItem-Identitäten und -Funktionen bereitstellen. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="f642c-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="f642c-110">Ordner haben ein [**„folder“-Facet**][-Ordner]</span><span class="sxs-lookup"><span data-stu-id="f642c-110">Folders have a [**folder facet**]</span></span>
* <span data-ttu-id="f642c-111">Dateien haben eine [**„file“-Facet**][-Datei].</span><span class="sxs-lookup"><span data-stu-id="f642c-111">Files have a [**file facet**].</span></span>
* <span data-ttu-id="f642c-112">Bilder haben zusätzlich zu ihrem „file“-Facet ein [**„image“Facet**][-Bild].</span><span class="sxs-lookup"><span data-stu-id="f642c-112">Images have an [**image facet**] in addition to their file facet.</span></span>
* <span data-ttu-id="f642c-113">Mit einer Kamera aufgenommene Bilder (Fotos) haben ein [**„photo“-Facet**][-Foto], das die Elemente als Foto identifiziert und als Eigenschaften das Aufnahmedatum sowie das zur Aufnahme verwendete Gerät aufführt.</span><span class="sxs-lookup"><span data-stu-id="f642c-113">Images taken with a camera (photos) have a [**photo facet**] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="f642c-114">Elemente mit dem **folder**-Facet fungieren als Elementcontainer und besitzen daher einen `children`-Verweis auf eine Sammlung von **driveItems** im jeweiligen Ordner.</span><span class="sxs-lookup"><span data-stu-id="f642c-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f642c-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f642c-115">JSON representation</span></span>

<span data-ttu-id="f642c-116">Es folgt eine JSON-Darstellung einer **driveItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="f642c-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="f642c-117">Die **driveItem**-Ressource wird von [**baseItem**][baseItem] abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="f642c-117">The **driveItem** resource is derived from [**baseItem**] and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
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
  "content": { "@odata.type": "Edm.Stream" },
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],

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

## <a name="properties"></a><span data-ttu-id="f642c-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f642c-118">Properties</span></span>

| <span data-ttu-id="f642c-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f642c-119">Property</span></span>             | <span data-ttu-id="f642c-120">Typ</span><span class="sxs-lookup"><span data-stu-id="f642c-120">Type</span></span>               | <span data-ttu-id="f642c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f642c-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="f642c-122">audio</span><span class="sxs-lookup"><span data-stu-id="f642c-122">audio</span></span>                | <span data-ttu-id="f642c-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="f642c-123">[audio][]</span></span>          | <span data-ttu-id="f642c-p103">Audiometadaten, wenn das Element eine Audiodatei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="f642c-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="f642c-126">createdBy</span></span>            | <span data-ttu-id="f642c-127">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f642c-127">[identitySet][]</span></span>    | <span data-ttu-id="f642c-p104">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="f642c-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f642c-130">createdDateTime</span></span>      | <span data-ttu-id="f642c-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f642c-131">DateTimeOffset</span></span>     | <span data-ttu-id="f642c-p105">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="f642c-134">cTag</span><span class="sxs-lookup"><span data-stu-id="f642c-134">cTag</span></span>                 | <span data-ttu-id="f642c-135">String</span><span class="sxs-lookup"><span data-stu-id="f642c-135">String</span></span>             | <span data-ttu-id="f642c-p106">Ein ETag für den Inhalt des Elements. Dieses ETag wird nicht geändert, wenn nur die Metadaten geändert werden. **Hinweis:** Diese Eigenschaft wird nicht zurückgegeben, wenn das Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="f642c-140">gelöscht</span><span class="sxs-lookup"><span data-stu-id="f642c-140">deleted</span></span>              | <span data-ttu-id="f642c-141">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="f642c-141">[deleted][]</span></span>        | <span data-ttu-id="f642c-p107">Informationen zum „gelöscht“-Zustand des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="f642c-144">description</span><span class="sxs-lookup"><span data-stu-id="f642c-144">description</span></span>          | <span data-ttu-id="f642c-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f642c-145">String</span></span>             | <span data-ttu-id="f642c-p108">Stellt eine für den Benutzer sichtbare Beschreibung des Elements bereit. Lese-/Schreibzugriff. Nur auf OneDrive Personal</span><span class="sxs-lookup"><span data-stu-id="f642c-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="f642c-149">eTag</span><span class="sxs-lookup"><span data-stu-id="f642c-149">eTag</span></span>                 | <span data-ttu-id="f642c-150">String</span><span class="sxs-lookup"><span data-stu-id="f642c-150">String</span></span>             | <span data-ttu-id="f642c-p109">ETag des gesamten Elements (Metadaten + Inhalt). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="f642c-153">file</span><span class="sxs-lookup"><span data-stu-id="f642c-153">file</span></span>                 | <span data-ttu-id="f642c-154">[file][]</span><span class="sxs-lookup"><span data-stu-id="f642c-154">[file][]</span></span>           | <span data-ttu-id="f642c-p110">Dateimetadaten, wenn das Element eine Datei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="f642c-157">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="f642c-157">fileSystemInfo</span></span>       | <span data-ttu-id="f642c-158">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="f642c-158">[fileSystemInfo][]</span></span> | <span data-ttu-id="f642c-p111">Informationen zum Dateisystem des Clients. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="f642c-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="f642c-161">folder</span><span class="sxs-lookup"><span data-stu-id="f642c-161">folder</span></span>               | <span data-ttu-id="f642c-162">[folder][]</span><span class="sxs-lookup"><span data-stu-id="f642c-162">[folder][]</span></span>         | <span data-ttu-id="f642c-p112">Ordnermetadaten, wenn das Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="f642c-165">id</span><span class="sxs-lookup"><span data-stu-id="f642c-165">id</span></span>                   | <span data-ttu-id="f642c-166">String</span><span class="sxs-lookup"><span data-stu-id="f642c-166">String</span></span>             | <span data-ttu-id="f642c-p113">Der eindeutige Bezeichner des Elements im Laufwerk. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="f642c-169">Abbildung</span><span class="sxs-lookup"><span data-stu-id="f642c-169">image</span></span>                | <span data-ttu-id="f642c-170">[image][]</span><span class="sxs-lookup"><span data-stu-id="f642c-170">[image][]</span></span>          | <span data-ttu-id="f642c-p114">Bildmetadaten, wenn das Element ein Bild ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="f642c-173">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f642c-173">lastModifiedBy</span></span>       | <span data-ttu-id="f642c-174">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f642c-174">[identitySet][]</span></span>    | <span data-ttu-id="f642c-p115">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="f642c-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f642c-177">lastModifiedDateTime</span></span> | <span data-ttu-id="f642c-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f642c-178">DateTimeOffset</span></span>     | <span data-ttu-id="f642c-p116">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f642c-181">location</span><span class="sxs-lookup"><span data-stu-id="f642c-181">location</span></span>             | <span data-ttu-id="f642c-182">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="f642c-182">[geoCoordinates][]</span></span> | <span data-ttu-id="f642c-p117">Standortmetadaten, sofern das Element Standortdaten aufweist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="f642c-185">name</span><span class="sxs-lookup"><span data-stu-id="f642c-185">name</span></span>                 | <span data-ttu-id="f642c-186">String</span><span class="sxs-lookup"><span data-stu-id="f642c-186">String</span></span>             | <span data-ttu-id="f642c-p118">Der Name des Elements (Dateiname und Erweiterung). Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="f642c-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="f642c-189">package</span><span class="sxs-lookup"><span data-stu-id="f642c-189">package</span></span>              | <span data-ttu-id="f642c-190">[package][]</span><span class="sxs-lookup"><span data-stu-id="f642c-190">[package][]</span></span>        | <span data-ttu-id="f642c-p119">Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="f642c-194">parentReference</span><span class="sxs-lookup"><span data-stu-id="f642c-194">parentReference</span></span>      | <span data-ttu-id="f642c-195">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="f642c-195">[itemReference][]</span></span>  | <span data-ttu-id="f642c-p120">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="f642c-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="f642c-198">Foto</span><span class="sxs-lookup"><span data-stu-id="f642c-198">photo</span></span>                | <span data-ttu-id="f642c-199">[photo][]</span><span class="sxs-lookup"><span data-stu-id="f642c-199">[photo][]</span></span>          | <span data-ttu-id="f642c-p121">Fotometadaten, wenn das Element ein Foto ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="f642c-202">remoteItem</span><span class="sxs-lookup"><span data-stu-id="f642c-202">remoteItem</span></span>           | <span data-ttu-id="f642c-203">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="f642c-203">[remoteItem][]</span></span>     | <span data-ttu-id="f642c-p122">Daten zum Remoteelement, wenn das Element von einem anderen Laufwerk freigegeben ist als dem, auf das zugegriffen wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p122">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="f642c-206">root</span><span class="sxs-lookup"><span data-stu-id="f642c-206">root</span></span>                 | <span data-ttu-id="f642c-207">[root][]</span><span class="sxs-lookup"><span data-stu-id="f642c-207">[root][]</span></span>           | <span data-ttu-id="f642c-208">Wenn diese Eigenschaft nicht Null ist, bedeutet dies, dass es sich bei der driveItem-Ressource um die oberste driveItem-Ressource auf dem Laufwerk handelt.</span><span class="sxs-lookup"><span data-stu-id="f642c-208">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="f642c-209">searchResult</span><span class="sxs-lookup"><span data-stu-id="f642c-209">searchResult</span></span>         | <span data-ttu-id="f642c-210">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="f642c-210">[searchResult][]</span></span>   | <span data-ttu-id="f642c-p123">Suchmetadaten, wenn das Element aus einem Suchergebnis stammt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p123">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="f642c-213">freigegeben</span><span class="sxs-lookup"><span data-stu-id="f642c-213">shared</span></span>               | <span data-ttu-id="f642c-214">[shared][]</span><span class="sxs-lookup"><span data-stu-id="f642c-214">[shared][]</span></span>         | <span data-ttu-id="f642c-p124">Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p124">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="f642c-217">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="f642c-217">sharepointIds</span></span>        | <span data-ttu-id="f642c-218">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f642c-218">[sharepointIds][]</span></span>  | <span data-ttu-id="f642c-p125">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p125">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="f642c-221">size</span><span class="sxs-lookup"><span data-stu-id="f642c-221">size</span></span>                 | <span data-ttu-id="f642c-222">Int64</span><span class="sxs-lookup"><span data-stu-id="f642c-222">Int64</span></span>              | <span data-ttu-id="f642c-p126">Größe des Elements in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p126">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="f642c-225">specialFolder</span><span class="sxs-lookup"><span data-stu-id="f642c-225">specialFolder</span></span>        | <span data-ttu-id="f642c-226">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="f642c-226">[specialFolder][]</span></span>  | <span data-ttu-id="f642c-p127">Facet, das zurückgegeben wird, wenn das aktuelle Element auch als spezieller Ordner verfügbar ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p127">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="f642c-229">video</span><span class="sxs-lookup"><span data-stu-id="f642c-229">video</span></span>                | <span data-ttu-id="f642c-230">[video][]</span><span class="sxs-lookup"><span data-stu-id="f642c-230">[video][]</span></span>          | <span data-ttu-id="f642c-p128">Videometadaten, wenn das Element ein Video ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p128">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="f642c-233">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="f642c-233">webDavUrl</span></span>            | <span data-ttu-id="f642c-234">String</span><span class="sxs-lookup"><span data-stu-id="f642c-234">String</span></span>             | <span data-ttu-id="f642c-235">WebDAV-kompatible URL für das Element.</span><span class="sxs-lookup"><span data-stu-id="f642c-235">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="f642c-236">webUrl</span><span class="sxs-lookup"><span data-stu-id="f642c-236">webUrl</span></span>               | <span data-ttu-id="f642c-237">String</span><span class="sxs-lookup"><span data-stu-id="f642c-237">String</span></span>             | <span data-ttu-id="f642c-p129">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p129">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="f642c-p130">**Hinweis:** Die Eigenschaften „eTag“ und „cTag“ arbeiten bei Containern (Ordnern) anders. Der Wert „cTag“ wird geändert, wenn Inhalte oder Metadaten eines Nachfolgers des Ordners geändert werden. Der Wert „eTag“ wird nur geändert, wenn die Eigenschaften des Ordners geändert werden. Ausnahme: Eigenschaften, die von Nachfolgern abgeleitet werden (wie **childCount** oder **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="f642c-p130">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="f642c-243">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f642c-243">Relationships</span></span>

| <span data-ttu-id="f642c-244">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f642c-244">Relationship</span></span>       | <span data-ttu-id="f642c-245">Typ</span><span class="sxs-lookup"><span data-stu-id="f642c-245">Type</span></span>                        | <span data-ttu-id="f642c-246">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f642c-246">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="f642c-247">Inhalt</span><span class="sxs-lookup"><span data-stu-id="f642c-247">content</span></span>            | <span data-ttu-id="f642c-248">Stream</span><span class="sxs-lookup"><span data-stu-id="f642c-248">Stream</span></span>                      | <span data-ttu-id="f642c-249">Der Inhaltsdatenstrom, wenn das Element eine Datei darstellt.</span><span class="sxs-lookup"><span data-stu-id="f642c-249">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="f642c-250">children</span><span class="sxs-lookup"><span data-stu-id="f642c-250">children</span></span>           | <span data-ttu-id="f642c-251">driveitem-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f642c-251">driveitem collection</span></span>        | <span data-ttu-id="f642c-p131">Sammlung von Elementobjekten der direkten untergeordneten Elemente eines Elements. Nur Elemente, die Ordner repräsentieren, haben untergeordnete Elemente. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f642c-p131">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="f642c-256">createdByUser</span><span class="sxs-lookup"><span data-stu-id="f642c-256">createdByUser</span></span>      | <span data-ttu-id="f642c-257">[user][]</span><span class="sxs-lookup"><span data-stu-id="f642c-257">[user][]</span></span>                    | <span data-ttu-id="f642c-258">Der Name des Benutzers, der das Element erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="f642c-258">Identity of the user who created the item.</span></span> <span data-ttu-id="f642c-259">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-259">Read-only.</span></span>
| <span data-ttu-id="f642c-260">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="f642c-260">lastModifiedByUser</span></span> | <span data-ttu-id="f642c-261">[user][]</span><span class="sxs-lookup"><span data-stu-id="f642c-261">[user][]</span></span>                    | <span data-ttu-id="f642c-262">Der Name des Benutzers, der das Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="f642c-262">Identity of the user, device, and application which last modified the item. Read-only.</span></span> <span data-ttu-id="f642c-263">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-263">Read-only.</span></span>
| <span data-ttu-id="f642c-264">permissions</span><span class="sxs-lookup"><span data-stu-id="f642c-264">permissions</span></span>        | <span data-ttu-id="f642c-265">[permission][] collection</span><span class="sxs-lookup"><span data-stu-id="f642c-265">[permission][] collection</span></span>   | <span data-ttu-id="f642c-p134">Der Satz von Berechtigungen für das Element. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f642c-p134">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="f642c-269">thumbnails</span><span class="sxs-lookup"><span data-stu-id="f642c-269">thumbnails</span></span>         | <span data-ttu-id="f642c-270">[thumbnailSet][] collection</span><span class="sxs-lookup"><span data-stu-id="f642c-270">[thumbnailSet][] collection</span></span> | <span data-ttu-id="f642c-p135">Sammlung der dem Element zugeordneten [ThumbnailSet][]-Objekte. Weitere Informationen finden Sie im Artikel zum [Abrufen von Miniaturansichten][]. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f642c-p135">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="f642c-275">Instanzenattribute</span><span class="sxs-lookup"><span data-stu-id="f642c-275">Instance Attributes</span></span>

<span data-ttu-id="f642c-p136">Instanzenattribute sind Eigenschaften mit speziellem Verhalten. Diese Eigenschaften sind temporär. Sie definieren entweder, wie sich der Dienst verhalten soll, oder geben kurzfristige Eigenschaftswerte an, beispielsweise URLs zum Elementdownload, die ablaufen.</span><span class="sxs-lookup"><span data-stu-id="f642c-p136">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="f642c-278">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="f642c-278">Property name</span></span>                     | <span data-ttu-id="f642c-279">Typ</span><span class="sxs-lookup"><span data-stu-id="f642c-279">Type</span></span>   | <span data-ttu-id="f642c-280">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f642c-280">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="f642c-281">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="f642c-281">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="f642c-282">string</span><span class="sxs-lookup"><span data-stu-id="f642c-282">string</span></span> | <span data-ttu-id="f642c-p137">Das Konfliktlösungsverhalten von Aktionen, die ein neues Element erstellen. Verwenden Sie die Werte *fail*, *replace* oder *rename*. Das Standardformat für PUT ist *replace*. Ein Element wird nie mit dieser Anmerkung zurückgegeben. Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="f642c-p137">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="f642c-288">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="f642c-288">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="f642c-289">string</span><span class="sxs-lookup"><span data-stu-id="f642c-289">string</span></span> | <span data-ttu-id="f642c-p138">Eine URL, über die die Inhalte der Datei heruntergeladen werden können. Eine Authentifizierung ist mit dieser URL nicht erforderlich. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f642c-p138">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="f642c-293">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="f642c-293">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="f642c-294">string</span><span class="sxs-lookup"><span data-stu-id="f642c-294">string</span></span> | <span data-ttu-id="f642c-p139">Bei Ausgabe einer PUT-Anforderung kann der Dienst mithilfe dieser Instanzanmerkung angewiesen werden, den Inhalt der URL herunterzuladen und als diese Datei zu speichern. Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="f642c-p139">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="f642c-p140">**Hinweis:** Der Wert „@microsoft.graph.downloadUrl“ ist eine kurzlebige URL und kann nicht zwischengespeichert werden. Die URL ist nur für kurze Zeit (1 Stunde) verfügbar, bevor sie ungültig wird.</span><span class="sxs-lookup"><span data-stu-id="f642c-p140">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached. The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>

## <a name="methods"></a><span data-ttu-id="f642c-299">Methoden</span><span class="sxs-lookup"><span data-stu-id="f642c-299">Methods</span></span>

| <span data-ttu-id="f642c-300">Method</span><span class="sxs-lookup"><span data-stu-id="f642c-300">Method</span></span>                                                   | <span data-ttu-id="f642c-301">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="f642c-301">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="f642c-302">Get item</span><span class="sxs-lookup"><span data-stu-id="f642c-302">Get item</span></span>](../api/driveitem_get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="f642c-303">List children</span><span class="sxs-lookup"><span data-stu-id="f642c-303">List children</span></span>](../api/driveitem_list_children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="f642c-304">Create item</span><span class="sxs-lookup"><span data-stu-id="f642c-304">Create item</span></span>](../api/driveitem_post_children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="f642c-305">Update item</span><span class="sxs-lookup"><span data-stu-id="f642c-305">Update item</span></span>](../api/driveitem_update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="f642c-306">Upload content</span><span class="sxs-lookup"><span data-stu-id="f642c-306">Upload content</span></span>](../api/driveitem_put_content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="f642c-307">Inhalte herunterladen</span><span class="sxs-lookup"><span data-stu-id="f642c-307">Download content</span></span>](../api/driveitem_get_content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="f642c-308">[Bestimmtes Dateiformat herunterladen][download-format]</span><span class="sxs-lookup"><span data-stu-id="f642c-308">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="f642c-309">Element löschen</span><span class="sxs-lookup"><span data-stu-id="f642c-309">Delete item</span></span>](../api/driveitem_delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="f642c-310">Move item</span><span class="sxs-lookup"><span data-stu-id="f642c-310">Move item</span></span>](../api/driveitem_move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="f642c-311">Copy item</span><span class="sxs-lookup"><span data-stu-id="f642c-311">Copy item</span></span>](../api/driveitem_copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="f642c-312">Search items</span><span class="sxs-lookup"><span data-stu-id="f642c-312">Search items</span></span>](../api/driveitem_search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="f642c-313">List changes in a drive</span><span class="sxs-lookup"><span data-stu-id="f642c-313">List changes in a drive</span></span>](../api/driveitem_delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="f642c-314">List thumbnails</span><span class="sxs-lookup"><span data-stu-id="f642c-314">List thumbnails</span></span>](../api/driveitem_list_thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="f642c-315">Create sharing link</span><span class="sxs-lookup"><span data-stu-id="f642c-315">Create sharing link</span></span>](../api/driveitem_createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="f642c-316">Add permissions</span><span class="sxs-lookup"><span data-stu-id="f642c-316">Add permissions</span></span>](../api/driveitem_invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="f642c-317">List permissions</span><span class="sxs-lookup"><span data-stu-id="f642c-317">List permissions</span></span>](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="f642c-318">Delete permission</span><span class="sxs-lookup"><span data-stu-id="f642c-318">Delete permission</span></span>](../api/permission_delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`


## <a name="remarks"></a><span data-ttu-id="f642c-319">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="f642c-319">Remarks</span></span>

<span data-ttu-id="f642c-320">In OneDrive for Business- oder SharePoint-Dokumentbibliotheken wird die Eigenschaft **cTag** nicht zurückgegeben, wenn die **driveItem**-Ressource ein [folder][]-Facet hat.</span><span class="sxs-lookup"><span data-stu-id="f642c-320">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseItem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem_get_content_format.md
[file]: file.md
[fileSystemInfo]: fileSystemInfo.md
[Ordner]: folder.md
[Abrufen von Miniaturansichten]: ../api/driveitem_list_thumbnails.md
[identitySet]: identitySet.md
[image]: image.md
[itemReference]: itemReference.md
[geoCoordinates]: geoCoordinates.md
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
[user]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/users

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
