---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: 13eb7ff286467a7acfef85f58ea59763a13d9801
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514334"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="bff45-102">RemoteItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bff45-102">RemoteItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bff45-p101">Die RemoteItem-Ressource gibt an, dass ein driveItem-Element auf ein Element in einem anderen Laufwerk verweist. Diese Ressource stellt die eindeutigen IDs des Quelllaufwerks und des Zielelements bereit.</span><span class="sxs-lookup"><span data-stu-id="bff45-p101">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="bff45-105">[**DriveItems**](driveitem.md) mit einem **remoteItem**-Facet ungleich Null sind Ressourcen, die freigegeben, zu OneDrive-Umgebungen von Benutzern hinzugefügt oder für Elemente von heterogenen Elementsammlungen (wie z. B. Suchergebnisse) zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="bff45-105">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="bff45-106">**Hinweis:** Im Gegensatz zu Ordnern im gleichen Laufwerk wird beim Verschieben eines **driveItem**-Elements in ein Remoteelement möglicherweise der `id`-Wert geändert.</span><span class="sxs-lookup"><span data-stu-id="bff45-106">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bff45-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bff45-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="bff45-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bff45-108">Properties</span></span>

| <span data-ttu-id="bff45-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="bff45-109">Property name</span></span>        | <span data-ttu-id="bff45-110">Typ</span><span class="sxs-lookup"><span data-stu-id="bff45-110">Type</span></span>                                | <span data-ttu-id="bff45-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bff45-111">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bff45-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="bff45-112">createdBy</span></span>            | [<span data-ttu-id="bff45-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="bff45-113">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="bff45-p102">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="bff45-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bff45-116">createdDateTime</span></span>      | <span data-ttu-id="bff45-117">Timestamp</span><span class="sxs-lookup"><span data-stu-id="bff45-117">Timestamp</span></span>                           | <span data-ttu-id="bff45-p103">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="bff45-120">file</span><span class="sxs-lookup"><span data-stu-id="bff45-120">file</span></span>                 | [<span data-ttu-id="bff45-121">Datei</span><span class="sxs-lookup"><span data-stu-id="bff45-121">File</span></span>](file.md)                     | <span data-ttu-id="bff45-p104">Gibt an, dass das Remote-Element eine Datei ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="bff45-124">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="bff45-124">fileSystemInfo</span></span>       | [<span data-ttu-id="bff45-125">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="bff45-125">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="bff45-p105">Informationen über das Remote-Element aus dem lokalen Dateisystem. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="bff45-128">folder</span><span class="sxs-lookup"><span data-stu-id="bff45-128">folder</span></span>               | [<span data-ttu-id="bff45-129">Ordner</span><span class="sxs-lookup"><span data-stu-id="bff45-129">Folder</span></span>](folder.md)                 | <span data-ttu-id="bff45-p106">Gibt an, dass das Remote-Element ein Ordner ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="bff45-132">id</span><span class="sxs-lookup"><span data-stu-id="bff45-132">id</span></span>                   | <span data-ttu-id="bff45-133">String</span><span class="sxs-lookup"><span data-stu-id="bff45-133">String</span></span>                              | <span data-ttu-id="bff45-p107">Eindeutige ID für das Remote-Element in dem Laufwerk. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="bff45-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="bff45-136">lastModifiedBy</span></span>       | [<span data-ttu-id="bff45-137">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="bff45-137">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="bff45-p108">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="bff45-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bff45-140">lastModifiedDateTime</span></span> | <span data-ttu-id="bff45-141">Timestamp</span><span class="sxs-lookup"><span data-stu-id="bff45-141">Timestamp</span></span>                           | <span data-ttu-id="bff45-p109">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="bff45-144">name</span><span class="sxs-lookup"><span data-stu-id="bff45-144">name</span></span>                 | <span data-ttu-id="bff45-145">String</span><span class="sxs-lookup"><span data-stu-id="bff45-145">String</span></span>                              | <span data-ttu-id="bff45-p110">Optional. Dateiname des Remote-Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="bff45-149">package</span><span class="sxs-lookup"><span data-stu-id="bff45-149">package</span></span>              | [<span data-ttu-id="bff45-150">Paket</span><span class="sxs-lookup"><span data-stu-id="bff45-150">Package</span></span>](package.md)               | <span data-ttu-id="bff45-p111">Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="bff45-154">parentReference</span><span class="sxs-lookup"><span data-stu-id="bff45-154">parentReference</span></span>      | [<span data-ttu-id="bff45-155">ItemReference</span><span class="sxs-lookup"><span data-stu-id="bff45-155">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="bff45-p112">Eigenschaften des übergeordneten Elements des Remote-Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="bff45-158">shared</span><span class="sxs-lookup"><span data-stu-id="bff45-158">shared</span></span>               | [<span data-ttu-id="bff45-159">shared</span><span class="sxs-lookup"><span data-stu-id="bff45-159">shared</span></span>](shared.md)                 | <span data-ttu-id="bff45-p113">Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="bff45-162">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="bff45-162">sharepointIds</span></span>        | [<span data-ttu-id="bff45-163">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="bff45-163">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="bff45-p114">Bietet Interoperabilität zwischen Elementen in OneDrive for Business und SharePoint mit vollständigem Satz an Element-IDs. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="bff45-166">size</span><span class="sxs-lookup"><span data-stu-id="bff45-166">size</span></span>                 | <span data-ttu-id="bff45-167">Int64</span><span class="sxs-lookup"><span data-stu-id="bff45-167">Int64</span></span>                               | <span data-ttu-id="bff45-p115">Größe des Remote-Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="bff45-170">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="bff45-170">webDavUrl</span></span>            | <span data-ttu-id="bff45-171">Url</span><span class="sxs-lookup"><span data-stu-id="bff45-171">Url</span></span>                                 | <span data-ttu-id="bff45-172">DAV-kompatible URL für das Element.</span><span class="sxs-lookup"><span data-stu-id="bff45-172">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="bff45-173">webUrl</span><span class="sxs-lookup"><span data-stu-id="bff45-173">webUrl</span></span>               | <span data-ttu-id="bff45-174">Url</span><span class="sxs-lookup"><span data-stu-id="bff45-174">Url</span></span>                                 | <span data-ttu-id="bff45-p116">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bff45-p116">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="bff45-177">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="bff45-177">Remarks</span></span>

<span data-ttu-id="bff45-178">Weitere Informationen über die Facets einer **driveItem**-Ressourcen finden Sie unter [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="bff45-178">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem",
  "suppressions": [
    "Error: /api-reference/beta/resources/remoteitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
