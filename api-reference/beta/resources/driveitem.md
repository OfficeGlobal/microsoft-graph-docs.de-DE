---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.openlocfilehash: 255b9de7ad565228da093a9a40d23c3360df28b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882264"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="8f2e1-102">Ressourcentyp driveItem</span><span class="sxs-lookup"><span data-stu-id="8f2e1-102">driveItem resource type</span></span>

> <span data-ttu-id="8f2e1-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f2e1-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f2e1-p102">Die **driveItem**-Ressource stellt eine Datei, einen Ordner oder ein anderes auf einem Laufwerk gespeichertes Element dar. Alle Dateisystemobjekte in OneDrive und SharePoint werden als **driveItem**-Ressourcen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p102">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="8f2e1-107">Es gibt zwei Hauptmethoden zum Adressieren einer **driveItem**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="8f2e1-107">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="8f2e1-108">Durch den eindeutigen **driveItem**-Bezeichner unter Verwendung von `drive/items/{item-id}`</span><span class="sxs-lookup"><span data-stu-id="8f2e1-108">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="8f2e1-109">Durch den Dateisystempfad unter Verwendung von `/drive/root:/path/to/file`</span><span class="sxs-lookup"><span data-stu-id="8f2e1-109">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="8f2e1-p103">**DriveItem**-Ressourcen verfügen über als Eigenschaften modellierte Facets, die Daten zu den driveItem-Identitäten und -Funktionen bereitstellen. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p103">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="8f2e1-112">Ordner haben ein [**„folder“-Facet**][-Ordner]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-112">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="8f2e1-113">Dateien haben eine [**„file“-Facet**][-Datei].</span><span class="sxs-lookup"><span data-stu-id="8f2e1-113">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="8f2e1-114">Bilder haben zusätzlich zu ihrem „file“-Facet ein [**„image“Facet**][-Bild].</span><span class="sxs-lookup"><span data-stu-id="8f2e1-114">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="8f2e1-115">Mit einer Kamera aufgenommene Bilder (Fotos) haben ein [**„photo“-Facet**][-Foto], das die Elemente als Foto identifiziert und als Eigenschaften das Aufnahmedatum sowie das zur Aufnahme verwendete Gerät aufführt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-115">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="8f2e1-116">Elemente mit dem **folder**-Facet fungieren als Elementcontainer und besitzen daher einen `children`-Verweis auf eine Sammlung von **driveItems** im jeweiligen Ordner.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-116">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f2e1-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f2e1-117">JSON representation</span></span>

<span data-ttu-id="8f2e1-118">Es folgt eine JSON-Darstellung einer **driveItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-118">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="8f2e1-119">Die **driveItem**-Ressource wird von [**baseItem**][baseItem] abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-119">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8f2e1-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f2e1-120">Properties</span></span>

| <span data-ttu-id="8f2e1-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f2e1-121">Property</span></span>             | <span data-ttu-id="8f2e1-122">Typ</span><span class="sxs-lookup"><span data-stu-id="8f2e1-122">Type</span></span>               | <span data-ttu-id="8f2e1-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f2e1-123">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="8f2e1-124">audio</span><span class="sxs-lookup"><span data-stu-id="8f2e1-124">audio</span></span>                | <span data-ttu-id="8f2e1-125">[audio][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-125">[audio][]</span></span>          | <span data-ttu-id="8f2e1-p104">Audiometadaten, wenn das Element eine Audiodatei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p104">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="8f2e1-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="8f2e1-128">createdBy</span></span>            | <span data-ttu-id="8f2e1-129">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-129">[identitySet][]</span></span>    | <span data-ttu-id="8f2e1-p105">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="8f2e1-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f2e1-132">createdDateTime</span></span>      | <span data-ttu-id="8f2e1-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f2e1-133">DateTimeOffset</span></span>     | <span data-ttu-id="8f2e1-p106">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p106">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="8f2e1-136">cTag</span><span class="sxs-lookup"><span data-stu-id="8f2e1-136">cTag</span></span>                 | <span data-ttu-id="8f2e1-137">String</span><span class="sxs-lookup"><span data-stu-id="8f2e1-137">String</span></span>             | <span data-ttu-id="8f2e1-p107">Ein ETag für den Inhalt des Elements. Dieses ETag wird nicht geändert, wenn nur die Metadaten geändert werden. **Hinweis:** Diese Eigenschaft wird nicht zurückgegeben, wenn das Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p107">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="8f2e1-142">gelöscht</span><span class="sxs-lookup"><span data-stu-id="8f2e1-142">deleted</span></span>              | <span data-ttu-id="8f2e1-143">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-143">[deleted][]</span></span>        | <span data-ttu-id="8f2e1-p108">Informationen zum „gelöscht“-Zustand des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p108">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="8f2e1-146">description</span><span class="sxs-lookup"><span data-stu-id="8f2e1-146">description</span></span>          | <span data-ttu-id="8f2e1-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f2e1-147">String</span></span>             | <span data-ttu-id="8f2e1-p109">Stellt eine für den Benutzer sichtbare Beschreibung des Elements bereit. Lese-/Schreibzugriff. Nur auf OneDrive Personal</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p109">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="8f2e1-151">eTag</span><span class="sxs-lookup"><span data-stu-id="8f2e1-151">eTag</span></span>                 | <span data-ttu-id="8f2e1-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f2e1-152">String</span></span>             | <span data-ttu-id="8f2e1-p110">ETag des gesamten Elements (Metadaten + Inhalt). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p110">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="8f2e1-155">file</span><span class="sxs-lookup"><span data-stu-id="8f2e1-155">file</span></span>                 | <span data-ttu-id="8f2e1-156">[file][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-156">[file][]</span></span>           | <span data-ttu-id="8f2e1-p111">Dateimetadaten, wenn das Element eine Datei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p111">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="8f2e1-159">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="8f2e1-159">fileSystemInfo</span></span>       | <span data-ttu-id="8f2e1-160">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-160">[fileSystemInfo][]</span></span> | <span data-ttu-id="8f2e1-p112">Informationen zum Dateisystem des Clients. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p112">File system information on client. Read-write.</span></span>
| <span data-ttu-id="8f2e1-163">folder</span><span class="sxs-lookup"><span data-stu-id="8f2e1-163">folder</span></span>               | <span data-ttu-id="8f2e1-164">[folder][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-164">[folder][]</span></span>         | <span data-ttu-id="8f2e1-p113">Ordnermetadaten, wenn das Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p113">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="8f2e1-167">id</span><span class="sxs-lookup"><span data-stu-id="8f2e1-167">id</span></span>                   | <span data-ttu-id="8f2e1-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f2e1-168">String</span></span>             | <span data-ttu-id="8f2e1-p114">Der eindeutige Bezeichner des Elements im Laufwerk. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p114">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="8f2e1-171">Abbildung</span><span class="sxs-lookup"><span data-stu-id="8f2e1-171">image</span></span>                | <span data-ttu-id="8f2e1-172">[image][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-172">[image][]</span></span>          | <span data-ttu-id="8f2e1-p115">Bildmetadaten, wenn das Element ein Bild ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p115">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="8f2e1-175">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8f2e1-175">lastModifiedBy</span></span>       | <span data-ttu-id="8f2e1-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-176">[identitySet][]</span></span>    | <span data-ttu-id="8f2e1-p116">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p116">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="8f2e1-179">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f2e1-179">lastModifiedDateTime</span></span> | <span data-ttu-id="8f2e1-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f2e1-180">DateTimeOffset</span></span>     | <span data-ttu-id="8f2e1-p117">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p117">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="8f2e1-183">location</span><span class="sxs-lookup"><span data-stu-id="8f2e1-183">location</span></span>             | <span data-ttu-id="8f2e1-184">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-184">[geoCoordinates][]</span></span> | <span data-ttu-id="8f2e1-p118">Standortmetadaten, sofern das Element Standortdaten aufweist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p118">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="8f2e1-187">name</span><span class="sxs-lookup"><span data-stu-id="8f2e1-187">name</span></span>                 | <span data-ttu-id="8f2e1-188">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f2e1-188">String</span></span>             | <span data-ttu-id="8f2e1-p119">Der Name des Elements (Dateiname und Erweiterung). Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p119">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="8f2e1-191">package</span><span class="sxs-lookup"><span data-stu-id="8f2e1-191">package</span></span>              | <span data-ttu-id="8f2e1-192">[package][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-192">[package][]</span></span>        | <span data-ttu-id="8f2e1-p120">Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p120">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="8f2e1-196">parentReference</span><span class="sxs-lookup"><span data-stu-id="8f2e1-196">parentReference</span></span>      | <span data-ttu-id="8f2e1-197">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-197">[itemReference][]</span></span>  | <span data-ttu-id="8f2e1-p121">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p121">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="8f2e1-200">Foto</span><span class="sxs-lookup"><span data-stu-id="8f2e1-200">photo</span></span>                | <span data-ttu-id="8f2e1-201">[photo][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-201">[photo][]</span></span>          | <span data-ttu-id="8f2e1-p122">Fotometadaten, wenn das Element ein Foto ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p122">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="8f2e1-204">Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="8f2e1-204">publication</span></span>          | <span data-ttu-id="8f2e1-205">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-205">[publicationFacet][]</span></span> | <span data-ttu-id="8f2e1-206">Stellt Informationen über den veröffentlichten oder ausgecheckten Status eines Elements an Stellen bereit, die solche Aktionen unterstützen.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-206">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="8f2e1-207">Diese Eigenschaft wird standardmäßig nicht zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-207">This property is not returned by default.</span></span> <span data-ttu-id="8f2e1-208">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-208">Read-only.</span></span> |
| <span data-ttu-id="8f2e1-209">remoteItem</span><span class="sxs-lookup"><span data-stu-id="8f2e1-209">remoteItem</span></span>           | <span data-ttu-id="8f2e1-210">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-210">[remoteItem][]</span></span>     | <span data-ttu-id="8f2e1-p124">Daten zum Remoteelement, wenn das Element von einem anderen Laufwerk freigegeben ist als dem, auf das zugegriffen wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p124">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="8f2e1-213">root</span><span class="sxs-lookup"><span data-stu-id="8f2e1-213">root</span></span>                 | <span data-ttu-id="8f2e1-214">[root][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-214">[root][]</span></span>           | <span data-ttu-id="8f2e1-215">Wenn diese Eigenschaft nicht Null ist, bedeutet dies, dass es sich bei der driveItem-Ressource um die oberste driveItem-Ressource auf dem Laufwerk handelt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-215">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="8f2e1-216">searchResult</span><span class="sxs-lookup"><span data-stu-id="8f2e1-216">searchResult</span></span>         | <span data-ttu-id="8f2e1-217">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-217">[searchResult][]</span></span>   | <span data-ttu-id="8f2e1-p125">Suchmetadaten, wenn das Element aus einem Suchergebnis stammt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p125">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="8f2e1-220">shared</span><span class="sxs-lookup"><span data-stu-id="8f2e1-220">shared</span></span>               | <span data-ttu-id="8f2e1-221">[shared][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-221">[shared][]</span></span>         | <span data-ttu-id="8f2e1-p126">Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p126">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="8f2e1-224">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="8f2e1-224">sharepointIds</span></span>        | <span data-ttu-id="8f2e1-225">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-225">[sharepointIds][]</span></span>  | <span data-ttu-id="8f2e1-p127">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p127">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="8f2e1-228">size</span><span class="sxs-lookup"><span data-stu-id="8f2e1-228">size</span></span>                 | <span data-ttu-id="8f2e1-229">Int64</span><span class="sxs-lookup"><span data-stu-id="8f2e1-229">Int64</span></span>              | <span data-ttu-id="8f2e1-p128">Größe des Elements in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p128">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="8f2e1-232">specialFolder</span><span class="sxs-lookup"><span data-stu-id="8f2e1-232">specialFolder</span></span>        | <span data-ttu-id="8f2e1-233">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-233">[specialFolder][]</span></span>  | <span data-ttu-id="8f2e1-p129">Facet, das zurückgegeben wird, wenn das aktuelle Element auch als spezieller Ordner verfügbar ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p129">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="8f2e1-236">video</span><span class="sxs-lookup"><span data-stu-id="8f2e1-236">video</span></span>                | <span data-ttu-id="8f2e1-237">[video][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-237">[video][]</span></span>          | <span data-ttu-id="8f2e1-p130">Videometadaten, wenn das Element ein Video ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p130">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="8f2e1-240">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="8f2e1-240">webDavUrl</span></span>            | <span data-ttu-id="8f2e1-241">String</span><span class="sxs-lookup"><span data-stu-id="8f2e1-241">String</span></span>             | <span data-ttu-id="8f2e1-242">WebDAV-kompatible URL für das Element.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-242">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="8f2e1-243">webUrl</span><span class="sxs-lookup"><span data-stu-id="8f2e1-243">webUrl</span></span>               | <span data-ttu-id="8f2e1-244">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f2e1-244">String</span></span>             | <span data-ttu-id="8f2e1-p131">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p131">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="8f2e1-p132">**Hinweis:** Die Eigenschaften „eTag“ und „cTag“ arbeiten bei Containern (Ordnern) anders. Der Wert „cTag“ wird geändert, wenn Inhalte oder Metadaten eines Nachfolgers des Ordners geändert werden. Der Wert „eTag“ wird nur geändert, wenn die Eigenschaften des Ordners geändert werden. Ausnahme: Eigenschaften, die von Nachfolgern abgeleitet werden (wie **childCount** oder **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p132">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="8f2e1-250">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8f2e1-250">Relationships</span></span>

| <span data-ttu-id="8f2e1-251">Beziehung</span><span class="sxs-lookup"><span data-stu-id="8f2e1-251">Relationship</span></span>       | <span data-ttu-id="8f2e1-252">Typ</span><span class="sxs-lookup"><span data-stu-id="8f2e1-252">Type</span></span>                            | <span data-ttu-id="8f2e1-253">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f2e1-253">Description</span></span>
|:-------------------|:--------------------------------|:--------------------------
| <span data-ttu-id="8f2e1-254">Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="8f2e1-254">activities</span></span>         | <span data-ttu-id="8f2e1-255">[ItemActivity][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8f2e1-255">[itemActivity][] collection</span></span>     | <span data-ttu-id="8f2e1-256">Die Liste der letzten Aktivitäten, die für dieses Element durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-256">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="8f2e1-257">Analytics</span><span class="sxs-lookup"><span data-stu-id="8f2e1-257">analytics</span></span>          | <span data-ttu-id="8f2e1-258">[ItemAnalytics][] -Ressource</span><span class="sxs-lookup"><span data-stu-id="8f2e1-258">[itemAnalytics][] resource</span></span>      | <span data-ttu-id="8f2e1-259">Analytics über die Aktivitäten anzeigen, die für dieses Element ausgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-259">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="8f2e1-260">content</span><span class="sxs-lookup"><span data-stu-id="8f2e1-260">content</span></span>            | <span data-ttu-id="8f2e1-261">Stream</span><span class="sxs-lookup"><span data-stu-id="8f2e1-261">Stream</span></span>                          | <span data-ttu-id="8f2e1-262">Der Inhaltsdatenstrom, wenn das Element eine Datei darstellt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-262">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="8f2e1-263">children</span><span class="sxs-lookup"><span data-stu-id="8f2e1-263">children</span></span>           | <span data-ttu-id="8f2e1-264">driveitem-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8f2e1-264">driveitem collection</span></span>            | <span data-ttu-id="8f2e1-p133">Sammlung von Elementobjekten der direkten untergeordneten Elemente eines Elements. Nur Elemente, die Ordner repräsentieren, haben untergeordnete Elemente. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p133">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="8f2e1-269">listItem</span><span class="sxs-lookup"><span data-stu-id="8f2e1-269">listItem</span></span>           | <span data-ttu-id="8f2e1-270">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-270">[listItem][]</span></span>                    | <span data-ttu-id="8f2e1-271">Für Laufwerke in SharePoint, die zugeordneten Dokumentbibliothek-Listenelement.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-271">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="8f2e1-272">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-272">Read-only.</span></span> <span data-ttu-id="8f2e1-273">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-273">Nullable.</span></span>
| <span data-ttu-id="8f2e1-274">permissions</span><span class="sxs-lookup"><span data-stu-id="8f2e1-274">permissions</span></span>        | <span data-ttu-id="8f2e1-275">[permission][] collection</span><span class="sxs-lookup"><span data-stu-id="8f2e1-275">[permission][] collection</span></span>       | <span data-ttu-id="8f2e1-p135">Der Satz von Berechtigungen für das Element. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p135">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="8f2e1-279">thumbnails</span><span class="sxs-lookup"><span data-stu-id="8f2e1-279">thumbnails</span></span>         | <span data-ttu-id="8f2e1-280">[thumbnailSet][] collection</span><span class="sxs-lookup"><span data-stu-id="8f2e1-280">[thumbnailSet][] collection</span></span>     | <span data-ttu-id="8f2e1-p136">Sammlung der dem Element zugeordneten [ThumbnailSet][]-Objekte. Weitere Informationen finden Sie im Artikel zum [Abrufen von Miniaturansichten][]. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p136">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="8f2e1-285">Versionen</span><span class="sxs-lookup"><span data-stu-id="8f2e1-285">versions</span></span>           | <span data-ttu-id="8f2e1-286">[DriveItemVersion][] -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8f2e1-286">[driveItemVersion][] collection</span></span> | <span data-ttu-id="8f2e1-287">Die Liste der vorherigen Versionen des Elements.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-287">The list of previous versions of the item.</span></span> <span data-ttu-id="8f2e1-288">Weitere Informationen finden Sie unter [Abrufen von früheren Versionen][].</span><span class="sxs-lookup"><span data-stu-id="8f2e1-288">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="8f2e1-289">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-289">Read-only.</span></span> <span data-ttu-id="8f2e1-290">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-290">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="8f2e1-291">Instanzenattribute</span><span class="sxs-lookup"><span data-stu-id="8f2e1-291">Instance Attributes</span></span>

<span data-ttu-id="8f2e1-p138">Instanzenattribute sind Eigenschaften mit speziellem Verhalten. Diese Eigenschaften sind temporär. Sie definieren entweder, wie sich der Dienst verhalten soll, oder geben kurzfristige Eigenschaftswerte an, beispielsweise URLs zum Elementdownload, die ablaufen.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p138">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="8f2e1-294">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="8f2e1-294">Property name</span></span>                     | <span data-ttu-id="8f2e1-295">Typ</span><span class="sxs-lookup"><span data-stu-id="8f2e1-295">Type</span></span>   | <span data-ttu-id="8f2e1-296">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f2e1-296">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="8f2e1-297">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="8f2e1-297">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="8f2e1-298">string</span><span class="sxs-lookup"><span data-stu-id="8f2e1-298">string</span></span> | <span data-ttu-id="8f2e1-p139">Das Konfliktlösungsverhalten von Aktionen, die ein neues Element erstellen. Verwenden Sie die Werte *fail*, *replace* oder *rename*. Das Standardformat für PUT ist *replace*. Ein Element wird nie mit dieser Anmerkung zurückgegeben. Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p139">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="8f2e1-304">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="8f2e1-304">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="8f2e1-305">string</span><span class="sxs-lookup"><span data-stu-id="8f2e1-305">string</span></span> | <span data-ttu-id="8f2e1-p140">Eine URL, über die die Inhalte der Datei heruntergeladen werden können. Eine Authentifizierung ist mit dieser URL nicht erforderlich. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p140">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="8f2e1-309">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="8f2e1-309">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="8f2e1-310">string</span><span class="sxs-lookup"><span data-stu-id="8f2e1-310">string</span></span> | <span data-ttu-id="8f2e1-p141">Bei Ausgabe einer PUT-Anforderung kann der Dienst mithilfe dieser Instanzanmerkung angewiesen werden, den Inhalt der URL herunterzuladen und als diese Datei zu speichern. Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-p141">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="8f2e1-313">**Hinweis:** Der @microsoft.graph.downloadUrl-Wert ist eine kurzlebige URL und kann nicht zwischengespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-313">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="8f2e1-314">Die URL ist verfügbar für einen kurzen Zeitraum (1 Stunde), bevor es ungültig ist.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-314">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span> <span data-ttu-id="8f2e1-315">Entfernen von Berechtigungen für einen Benutzer möglicherweise die URL nicht sofort ungültig.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-315">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

## <a name="methods"></a><span data-ttu-id="8f2e1-316">Methoden</span><span class="sxs-lookup"><span data-stu-id="8f2e1-316">Methods</span></span>

| <span data-ttu-id="8f2e1-317">Methode</span><span class="sxs-lookup"><span data-stu-id="8f2e1-317">Method</span></span>                                                   | <span data-ttu-id="8f2e1-318">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="8f2e1-318">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="8f2e1-319">Element abrufen</span><span class="sxs-lookup"><span data-stu-id="8f2e1-319">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="8f2e1-320">Aktivitäten auflisten</span><span class="sxs-lookup"><span data-stu-id="8f2e1-320">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="8f2e1-321">[Abrufen von analytics][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-321">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="8f2e1-322">[Abrufen von Aktivitäten nach Intervall][]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-322">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="8f2e1-323">Untergeordnete Objekte auflisten</span><span class="sxs-lookup"><span data-stu-id="8f2e1-323">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="8f2e1-324">Versionen auflisten</span><span class="sxs-lookup"><span data-stu-id="8f2e1-324">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="8f2e1-325">Create item</span><span class="sxs-lookup"><span data-stu-id="8f2e1-325">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="8f2e1-326">Update item</span><span class="sxs-lookup"><span data-stu-id="8f2e1-326">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="8f2e1-327">Upload content</span><span class="sxs-lookup"><span data-stu-id="8f2e1-327">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="8f2e1-328">Inhalte herunterladen</span><span class="sxs-lookup"><span data-stu-id="8f2e1-328">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="8f2e1-329">[Bestimmtes Dateiformat herunterladen][download-format]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-329">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="8f2e1-330">Element löschen</span><span class="sxs-lookup"><span data-stu-id="8f2e1-330">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="8f2e1-331">Move item</span><span class="sxs-lookup"><span data-stu-id="8f2e1-331">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="8f2e1-332">Copy item</span><span class="sxs-lookup"><span data-stu-id="8f2e1-332">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="8f2e1-333">Search items</span><span class="sxs-lookup"><span data-stu-id="8f2e1-333">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="8f2e1-334">List changes in a drive</span><span class="sxs-lookup"><span data-stu-id="8f2e1-334">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="8f2e1-335">List thumbnails</span><span class="sxs-lookup"><span data-stu-id="8f2e1-335">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="8f2e1-336">Freigabelink erstellen</span><span class="sxs-lookup"><span data-stu-id="8f2e1-336">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="8f2e1-337">Berechtigungen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="8f2e1-337">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="8f2e1-338">Berechtigungen auflisten</span><span class="sxs-lookup"><span data-stu-id="8f2e1-338">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="8f2e1-339">Delete permission</span><span class="sxs-lookup"><span data-stu-id="8f2e1-339">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="8f2e1-340">[DDE-Kanal WebSocket abrufen][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-340">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="8f2e1-341">[Preview-Element][item-preview]</span><span class="sxs-lookup"><span data-stu-id="8f2e1-341">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[Abrufen von analytics]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Abrufen von Aktivitäten nach Intervall]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="8f2e1-344">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="8f2e1-344">Remarks</span></span>

<span data-ttu-id="8f2e1-345">In OneDrive for Business- oder SharePoint-Dokumentbibliotheken wird die Eigenschaft **cTag** nicht zurückgegeben, wenn die **driveItem**-Ressource ein [Ordner][]-Facet hat.</span><span class="sxs-lookup"><span data-stu-id="8f2e1-345">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
