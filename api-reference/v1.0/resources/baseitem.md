---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
ms.openlocfilehash: bbfebd734407259c391cdb1ce74beb96dc74d8bf
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="c29c4-102">baseItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c29c4-102">BaseItem resource type</span></span>

<span data-ttu-id="c29c4-p101">Die **baseItem**-Ressource ist eine abstrakte Ressource, die einen gemeinsamen Satz von Eigenschaften enthält, die auch von mehreren anderen Ressourcen verwendet werden. Folgende Ressourcen werden u. a. von abgeleitet **baseItem** abgeleitet:</span><span class="sxs-lookup"><span data-stu-id="c29c4-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="c29c4-105">Laufwerk</span><span class="sxs-lookup"><span data-stu-id="c29c4-105">drive</span></span>](drive.md)
* [<span data-ttu-id="c29c4-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="c29c4-106">DriveItem</span></span>](driveitem.md)
* [<span data-ttu-id="c29c4-107">site</span><span class="sxs-lookup"><span data-stu-id="c29c4-107">site</span></span>](site.md)
* [<span data-ttu-id="c29c4-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="c29c4-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="c29c4-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c29c4-109">JSON representation</span></span>

<span data-ttu-id="c29c4-110">Es folgt eine JSON-Darstellung einer **baseItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="c29c4-110">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c29c4-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c29c4-111">Properties</span></span>

| <span data-ttu-id="c29c4-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c29c4-112">Property</span></span>             | <span data-ttu-id="c29c4-113">Typ</span><span class="sxs-lookup"><span data-stu-id="c29c4-113">Type</span></span>              | <span data-ttu-id="c29c4-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c29c4-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="c29c4-115">id</span><span class="sxs-lookup"><span data-stu-id="c29c4-115">id</span></span>                   | <span data-ttu-id="c29c4-116">string</span><span class="sxs-lookup"><span data-stu-id="c29c4-116">string</span></span>            | <span data-ttu-id="c29c4-p102">Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c29c4-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="c29c4-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="c29c4-119">createdBy</span></span>            | <span data-ttu-id="c29c4-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c29c4-120">[identitySet][]</span></span>   | <span data-ttu-id="c29c4-p103">Die Identität des Benutzers, des Geräts oder der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c29c4-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="c29c4-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c29c4-123">createdDateTime</span></span>      | <span data-ttu-id="c29c4-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c29c4-124">dateTimeOffset</span></span>    | <span data-ttu-id="c29c4-p104">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c29c4-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="c29c4-127">eTag</span><span class="sxs-lookup"><span data-stu-id="c29c4-127">eTag</span></span>                 | <span data-ttu-id="c29c4-128">string</span><span class="sxs-lookup"><span data-stu-id="c29c4-128">string</span></span>            | <span data-ttu-id="c29c4-p105">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c29c4-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="c29c4-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c29c4-131">lastModifiedBy</span></span>       | <span data-ttu-id="c29c4-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c29c4-132">[identitySet][]</span></span>   | <span data-ttu-id="c29c4-p106">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c29c4-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="c29c4-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c29c4-135">lastModifiedDateTime</span></span> | <span data-ttu-id="c29c4-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c29c4-136">dateTimeOffset</span></span>    | <span data-ttu-id="c29c4-p107">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c29c4-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="c29c4-139">name</span><span class="sxs-lookup"><span data-stu-id="c29c4-139">name</span></span>                 | <span data-ttu-id="c29c4-140">string</span><span class="sxs-lookup"><span data-stu-id="c29c4-140">string</span></span>            | <span data-ttu-id="c29c4-p108">Der Name des Elements. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="c29c4-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="c29c4-143">parentReference</span><span class="sxs-lookup"><span data-stu-id="c29c4-143">parentReference</span></span>      | <span data-ttu-id="c29c4-144">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="c29c4-144">[itemReference][]</span></span> | <span data-ttu-id="c29c4-p109">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="c29c4-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="c29c4-147">webUrl</span><span class="sxs-lookup"><span data-stu-id="c29c4-147">webUrl</span></span>               | <span data-ttu-id="c29c4-148">String (URL)</span><span class="sxs-lookup"><span data-stu-id="c29c4-148">string (url)</span></span>      | <span data-ttu-id="c29c4-p110">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c29c4-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="c29c4-153">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="c29c4-153">Remarks</span></span>

<span data-ttu-id="c29c4-154">Der Typ `baseItem` wird voraussichtlich nicht direkt verwendet.</span><span class="sxs-lookup"><span data-stu-id="c29c4-154">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
