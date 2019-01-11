---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: 0b29ba14273bad7306518c290029a9ebc444f07d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888088"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="ec1c5-102">RemoteItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ec1c5-102">RemoteItem resource type</span></span>

<span data-ttu-id="ec1c5-p101">Die **RemoteItem**-Ressource gibt an, dass ein [**driveItem**](driveitem.md)-Element auf ein Element in einem anderen Laufwerk verweist. Diese Ressource stellt die eindeutigen IDs des Quelllaufwerks und des Zielelements bereit.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p101">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="ec1c5-105">[**DriveItems**](driveitem.md) mit einem **remoteItem**-Facet ungleich Null sind Ressourcen, die freigegeben, zu OneDrive-Umgebungen von Benutzern hinzugefügt oder für Elemente von heterogenen Elementsammlungen (wie z. B. Suchergebnisse) zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-105">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="ec1c5-106">**Hinweis:** Im Gegensatz zu Ordnern im gleichen Laufwerk wird beim Verschieben eines **driveItem**-Elements in ein Remoteelement möglicherweise der `id`-Wert geändert.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-106">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec1c5-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ec1c5-107">JSON representation</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.remoteItem", 
       "optionalProperties": ["name", "fileSystemInfo", "file", "folder"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="ec1c5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ec1c5-108">Properties</span></span>

| <span data-ttu-id="ec1c5-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="ec1c5-109">Property name</span></span>        | <span data-ttu-id="ec1c5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ec1c5-110">Type</span></span>                                | <span data-ttu-id="ec1c5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec1c5-111">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ec1c5-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="ec1c5-112">createdBy</span></span>            | [<span data-ttu-id="ec1c5-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="ec1c5-113">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="ec1c5-p102">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="ec1c5-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec1c5-116">createdDateTime</span></span>      | <span data-ttu-id="ec1c5-117">Timestamp</span><span class="sxs-lookup"><span data-stu-id="ec1c5-117">Timestamp</span></span>                           | <span data-ttu-id="ec1c5-p103">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="ec1c5-120">file</span><span class="sxs-lookup"><span data-stu-id="ec1c5-120">file</span></span>                 | [<span data-ttu-id="ec1c5-121">Datei</span><span class="sxs-lookup"><span data-stu-id="ec1c5-121">File</span></span>](file.md)                     | <span data-ttu-id="ec1c5-p104">Gibt an, dass das Remote-Element eine Datei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="ec1c5-124">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="ec1c5-124">fileSystemInfo</span></span>       | [<span data-ttu-id="ec1c5-125">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="ec1c5-125">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="ec1c5-p105">Informationen über das Remote-Element aus dem lokalen Dateisystem. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="ec1c5-128">folder</span><span class="sxs-lookup"><span data-stu-id="ec1c5-128">folder</span></span>               | [<span data-ttu-id="ec1c5-129">Ordner</span><span class="sxs-lookup"><span data-stu-id="ec1c5-129">Folder</span></span>](folder.md)                 | <span data-ttu-id="ec1c5-p106">Gibt an, dass das Remote-Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="ec1c5-132">id</span><span class="sxs-lookup"><span data-stu-id="ec1c5-132">id</span></span>                   | <span data-ttu-id="ec1c5-133">String</span><span class="sxs-lookup"><span data-stu-id="ec1c5-133">String</span></span>                              | <span data-ttu-id="ec1c5-p107">Eindeutige ID für das Remote-Element in dem Laufwerk. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="ec1c5-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ec1c5-136">lastModifiedBy</span></span>       | [<span data-ttu-id="ec1c5-137">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="ec1c5-137">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="ec1c5-p108">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="ec1c5-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec1c5-140">lastModifiedDateTime</span></span> | <span data-ttu-id="ec1c5-141">Timestamp</span><span class="sxs-lookup"><span data-stu-id="ec1c5-141">Timestamp</span></span>                           | <span data-ttu-id="ec1c5-p109">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="ec1c5-144">name</span><span class="sxs-lookup"><span data-stu-id="ec1c5-144">name</span></span>                 | <span data-ttu-id="ec1c5-145">String</span><span class="sxs-lookup"><span data-stu-id="ec1c5-145">String</span></span>                              | <span data-ttu-id="ec1c5-p110">Optional. Dateiname des Remote-Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="ec1c5-149">package</span><span class="sxs-lookup"><span data-stu-id="ec1c5-149">package</span></span>              | [<span data-ttu-id="ec1c5-150">Paket</span><span class="sxs-lookup"><span data-stu-id="ec1c5-150">Package</span></span>](package.md)               | <span data-ttu-id="ec1c5-p111">Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="ec1c5-154">parentReference</span><span class="sxs-lookup"><span data-stu-id="ec1c5-154">parentReference</span></span>      | [<span data-ttu-id="ec1c5-155">ItemReference</span><span class="sxs-lookup"><span data-stu-id="ec1c5-155">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="ec1c5-p112">Eigenschaften des übergeordneten Elements des Remote-Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="ec1c5-158">shared</span><span class="sxs-lookup"><span data-stu-id="ec1c5-158">shared</span></span>               | [<span data-ttu-id="ec1c5-159">shared</span><span class="sxs-lookup"><span data-stu-id="ec1c5-159">shared</span></span>](shared.md)                 | <span data-ttu-id="ec1c5-p113">Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="ec1c5-162">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ec1c5-162">sharepointIds</span></span>        | [<span data-ttu-id="ec1c5-163">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="ec1c5-163">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="ec1c5-p114">Bietet Interoperabilität zwischen Elementen in OneDrive for Business und SharePoint mit vollständigem Satz an Element-IDs. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="ec1c5-166">size</span><span class="sxs-lookup"><span data-stu-id="ec1c5-166">size</span></span>                 | <span data-ttu-id="ec1c5-167">Int64</span><span class="sxs-lookup"><span data-stu-id="ec1c5-167">Int64</span></span>                               | <span data-ttu-id="ec1c5-p115">Größe des Remote-Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="ec1c5-170">specialFolder</span><span class="sxs-lookup"><span data-stu-id="ec1c5-170">specialFolder</span></span>        | <span data-ttu-id="ec1c5-171">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="ec1c5-171">[specialFolder][]</span></span>                   | <span data-ttu-id="ec1c5-p116">Facet, das zurückgegeben wird, wenn das aktuelle Element auch als spezieller Ordner verfügbar ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p116">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>                                                                     |
| <span data-ttu-id="ec1c5-174">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="ec1c5-174">webDavUrl</span></span>            | <span data-ttu-id="ec1c5-175">Url</span><span class="sxs-lookup"><span data-stu-id="ec1c5-175">Url</span></span>                                 | <span data-ttu-id="ec1c5-176">DAV-kompatible URL für das Element.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-176">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="ec1c5-177">webUrl</span><span class="sxs-lookup"><span data-stu-id="ec1c5-177">webUrl</span></span>               | <span data-ttu-id="ec1c5-178">Url</span><span class="sxs-lookup"><span data-stu-id="ec1c5-178">Url</span></span>                                 | <span data-ttu-id="ec1c5-p117">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ec1c5-p117">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

[specialFolder]: specialfolder.md

## <a name="remarks"></a><span data-ttu-id="ec1c5-182">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="ec1c5-182">Remarks</span></span>

<span data-ttu-id="ec1c5-183">Weitere Informationen über die Facets einer **driveItem**-Ressourcen finden Sie unter [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ec1c5-183">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
