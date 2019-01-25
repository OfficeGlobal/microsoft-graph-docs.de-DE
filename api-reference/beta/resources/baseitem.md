---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: 5bc3aab8460c1d0c6774d2f8afda13c4fc89f69d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521586"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="f1995-102">baseItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f1995-102">BaseItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1995-p101">Die **baseItem**-Ressource ist eine abstrakte Ressource, die einen gemeinsamen Satz von Eigenschaften enthält, die auch von mehreren anderen Ressourcen verwendet werden. Folgende Ressourcen werden u. a. von abgeleitet **baseItem** abgeleitet:</span><span class="sxs-lookup"><span data-stu-id="f1995-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="f1995-105">Laufwerk</span><span class="sxs-lookup"><span data-stu-id="f1995-105">drive</span></span>](drive.md)
* [<span data-ttu-id="f1995-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="f1995-106">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="f1995-107">site</span><span class="sxs-lookup"><span data-stu-id="f1995-107">site</span></span>](site.md)
* [<span data-ttu-id="f1995-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="f1995-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="f1995-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f1995-109">JSON representation</span></span>

<span data-ttu-id="f1995-110">Es folgt eine JSON-Darstellung einer **baseItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="f1995-110">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem"
}-->

```json
{
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="f1995-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f1995-111">Properties</span></span>

| <span data-ttu-id="f1995-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1995-112">Property</span></span>             | <span data-ttu-id="f1995-113">Typ</span><span class="sxs-lookup"><span data-stu-id="f1995-113">Type</span></span>              | <span data-ttu-id="f1995-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1995-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="f1995-115">id</span><span class="sxs-lookup"><span data-stu-id="f1995-115">id</span></span>                   | <span data-ttu-id="f1995-116">string</span><span class="sxs-lookup"><span data-stu-id="f1995-116">string</span></span>            | <span data-ttu-id="f1995-p102">Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f1995-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="f1995-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="f1995-119">createdBy</span></span>            | <span data-ttu-id="f1995-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f1995-120">[identitySet][]</span></span>   | <span data-ttu-id="f1995-p103">Die Identität des Benutzers, des Geräts oder der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f1995-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="f1995-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1995-123">createdDateTime</span></span>      | <span data-ttu-id="f1995-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1995-124">dateTimeOffset</span></span>    | <span data-ttu-id="f1995-p104">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f1995-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="f1995-127">eTag</span><span class="sxs-lookup"><span data-stu-id="f1995-127">eTag</span></span>                 | <span data-ttu-id="f1995-128">string</span><span class="sxs-lookup"><span data-stu-id="f1995-128">string</span></span>            | <span data-ttu-id="f1995-p105">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f1995-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="f1995-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f1995-131">lastModifiedBy</span></span>       | <span data-ttu-id="f1995-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f1995-132">[identitySet][]</span></span>   | <span data-ttu-id="f1995-p106">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f1995-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="f1995-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1995-135">lastModifiedDateTime</span></span> | <span data-ttu-id="f1995-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1995-136">dateTimeOffset</span></span>    | <span data-ttu-id="f1995-p107">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f1995-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="f1995-139">name</span><span class="sxs-lookup"><span data-stu-id="f1995-139">name</span></span>                 | <span data-ttu-id="f1995-140">string</span><span class="sxs-lookup"><span data-stu-id="f1995-140">string</span></span>            | <span data-ttu-id="f1995-p108">Der Name des Elements. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="f1995-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="f1995-143">parentReference</span><span class="sxs-lookup"><span data-stu-id="f1995-143">parentReference</span></span>      | <span data-ttu-id="f1995-144">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="f1995-144">[itemReference][]</span></span> | <span data-ttu-id="f1995-p109">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="f1995-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="f1995-147">webUrl</span><span class="sxs-lookup"><span data-stu-id="f1995-147">webUrl</span></span>               | <span data-ttu-id="f1995-148">String (URL)</span><span class="sxs-lookup"><span data-stu-id="f1995-148">string (url)</span></span>      | <span data-ttu-id="f1995-p110">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f1995-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="f1995-153">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="f1995-153">Remarks</span></span>

<span data-ttu-id="f1995-154">Der Typ `baseItem` wird voraussichtlich nicht direkt verwendet.</span><span class="sxs-lookup"><span data-stu-id="f1995-154">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
