---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: 122e13513db1a59e23a41cadd16e61996e6a6c04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843190"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="733a7-102">RemoteItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="733a7-102">RemoteItem resource type</span></span>

> <span data-ttu-id="733a7-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="733a7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="733a7-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="733a7-p102">Die **RemoteItem**-Ressource gibt an, dass ein [**driveItem**](driveitem.md)-Element auf ein Element in einem anderen Laufwerk verweist. Diese Ressource stellt die eindeutigen IDs des Quelllaufwerks und des Zielelements bereit.</span><span class="sxs-lookup"><span data-stu-id="733a7-p102">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="733a7-107">[**DriveItems**](driveitem.md) mit einem **remoteItem**-Facet ungleich Null sind Ressourcen, die freigegeben, zu OneDrive-Umgebungen von Benutzern hinzugefügt oder für Elemente von heterogenen Elementsammlungen (wie z. B. Suchergebnisse) zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="733a7-107">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="733a7-108">**Hinweis:** Im Gegensatz zu Ordnern im gleichen Laufwerk wird beim Verschieben eines **driveItem**-Elements in ein Remoteelement möglicherweise der `id`-Wert geändert.</span><span class="sxs-lookup"><span data-stu-id="733a7-108">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="733a7-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="733a7-109">JSON representation</span></span>

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
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="733a7-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="733a7-110">Properties</span></span>

| <span data-ttu-id="733a7-111">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="733a7-111">Property name</span></span>        | <span data-ttu-id="733a7-112">Typ</span><span class="sxs-lookup"><span data-stu-id="733a7-112">Type</span></span>                                | <span data-ttu-id="733a7-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="733a7-113">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="733a7-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="733a7-114">createdBy</span></span>            | [<span data-ttu-id="733a7-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="733a7-115">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="733a7-p103">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="733a7-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="733a7-118">createdDateTime</span></span>      | <span data-ttu-id="733a7-119">Timestamp</span><span class="sxs-lookup"><span data-stu-id="733a7-119">Timestamp</span></span>                           | <span data-ttu-id="733a7-p104">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="733a7-122">file</span><span class="sxs-lookup"><span data-stu-id="733a7-122">file</span></span>                 | [<span data-ttu-id="733a7-123">File</span><span class="sxs-lookup"><span data-stu-id="733a7-123">File</span></span>](file.md)                     | <span data-ttu-id="733a7-p105">Gibt an, dass das Remote-Element eine Datei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p105">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="733a7-126">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="733a7-126">fileSystemInfo</span></span>       | [<span data-ttu-id="733a7-127">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="733a7-127">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="733a7-p106">Informationen über das Remote-Element aus dem lokalen Dateisystem. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p106">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="733a7-130">folder</span><span class="sxs-lookup"><span data-stu-id="733a7-130">folder</span></span>               | [<span data-ttu-id="733a7-131">Ordner</span><span class="sxs-lookup"><span data-stu-id="733a7-131">Folder</span></span>](folder.md)                 | <span data-ttu-id="733a7-p107">Gibt an, dass das Remote-Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p107">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="733a7-134">id</span><span class="sxs-lookup"><span data-stu-id="733a7-134">id</span></span>                   | <span data-ttu-id="733a7-135">String</span><span class="sxs-lookup"><span data-stu-id="733a7-135">String</span></span>                              | <span data-ttu-id="733a7-p108">Eindeutige ID für das Remote-Element in dem Laufwerk. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p108">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="733a7-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="733a7-138">lastModifiedBy</span></span>       | [<span data-ttu-id="733a7-139">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="733a7-139">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="733a7-p109">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p109">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="733a7-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="733a7-142">lastModifiedDateTime</span></span> | <span data-ttu-id="733a7-143">Timestamp</span><span class="sxs-lookup"><span data-stu-id="733a7-143">Timestamp</span></span>                           | <span data-ttu-id="733a7-p110">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p110">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="733a7-146">name</span><span class="sxs-lookup"><span data-stu-id="733a7-146">name</span></span>                 | <span data-ttu-id="733a7-147">String</span><span class="sxs-lookup"><span data-stu-id="733a7-147">String</span></span>                              | <span data-ttu-id="733a7-p111">Optional. Dateiname des Remote-Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p111">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="733a7-151">package</span><span class="sxs-lookup"><span data-stu-id="733a7-151">package</span></span>              | [<span data-ttu-id="733a7-152">Paket</span><span class="sxs-lookup"><span data-stu-id="733a7-152">Package</span></span>](package.md)               | <span data-ttu-id="733a7-p112">Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p112">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="733a7-156">parentReference</span><span class="sxs-lookup"><span data-stu-id="733a7-156">parentReference</span></span>      | [<span data-ttu-id="733a7-157">ItemReference</span><span class="sxs-lookup"><span data-stu-id="733a7-157">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="733a7-p113">Eigenschaften des übergeordneten Elements des Remote-Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p113">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="733a7-160">shared</span><span class="sxs-lookup"><span data-stu-id="733a7-160">shared</span></span>               | [<span data-ttu-id="733a7-161">shared</span><span class="sxs-lookup"><span data-stu-id="733a7-161">shared</span></span>](shared.md)                 | <span data-ttu-id="733a7-p114">Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p114">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="733a7-164">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="733a7-164">sharepointIds</span></span>        | [<span data-ttu-id="733a7-165">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="733a7-165">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="733a7-p115">Bietet Interoperabilität zwischen Elementen in OneDrive for Business und SharePoint mit vollständigem Satz an Element-IDs. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p115">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="733a7-168">size</span><span class="sxs-lookup"><span data-stu-id="733a7-168">size</span></span>                 | <span data-ttu-id="733a7-169">Int64</span><span class="sxs-lookup"><span data-stu-id="733a7-169">Int64</span></span>                               | <span data-ttu-id="733a7-p116">Größe des Remote-Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p116">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="733a7-172">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="733a7-172">webDavUrl</span></span>            | <span data-ttu-id="733a7-173">Url</span><span class="sxs-lookup"><span data-stu-id="733a7-173">Url</span></span>                                 | <span data-ttu-id="733a7-174">DAV-kompatible URL für das Element.</span><span class="sxs-lookup"><span data-stu-id="733a7-174">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="733a7-175">webUrl</span><span class="sxs-lookup"><span data-stu-id="733a7-175">webUrl</span></span>               | <span data-ttu-id="733a7-176">Url</span><span class="sxs-lookup"><span data-stu-id="733a7-176">Url</span></span>                                 | <span data-ttu-id="733a7-p117">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="733a7-p117">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="733a7-179">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="733a7-179">Remarks</span></span>

<span data-ttu-id="733a7-180">Weitere Informationen über die Facets einer **driveItem**-Ressourcen finden Sie unter [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="733a7-180">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
