---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: ac119ab0b63aecba384d34014f3d0d18111b05ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866248"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="0dd5a-102">baseItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0dd5a-102">BaseItem resource type</span></span>

> <span data-ttu-id="0dd5a-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0dd5a-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0dd5a-p102">Die **baseItem**-Ressource ist eine abstrakte Ressource, die einen gemeinsamen Satz von Eigenschaften enthält, die auch von mehreren anderen Ressourcen verwendet werden. Folgende Ressourcen werden u. a. von abgeleitet **baseItem** abgeleitet:</span><span class="sxs-lookup"><span data-stu-id="0dd5a-p102">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="0dd5a-107">Laufwerk</span><span class="sxs-lookup"><span data-stu-id="0dd5a-107">drive</span></span>](drive.md)
* [<span data-ttu-id="0dd5a-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="0dd5a-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="0dd5a-109">site</span><span class="sxs-lookup"><span data-stu-id="0dd5a-109">site</span></span>](site.md)
* [<span data-ttu-id="0dd5a-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="0dd5a-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="0dd5a-111">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0dd5a-111">JSON representation</span></span>

<span data-ttu-id="0dd5a-112">Es folgt eine JSON-Darstellung einer **baseItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-112">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0dd5a-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0dd5a-113">Properties</span></span>

| <span data-ttu-id="0dd5a-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0dd5a-114">Property</span></span>             | <span data-ttu-id="0dd5a-115">Typ</span><span class="sxs-lookup"><span data-stu-id="0dd5a-115">Type</span></span>              | <span data-ttu-id="0dd5a-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0dd5a-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="0dd5a-117">id</span><span class="sxs-lookup"><span data-stu-id="0dd5a-117">id</span></span>                   | <span data-ttu-id="0dd5a-118">string</span><span class="sxs-lookup"><span data-stu-id="0dd5a-118">string</span></span>            | <span data-ttu-id="0dd5a-p103">Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-p103">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="0dd5a-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="0dd5a-121">createdBy</span></span>            | <span data-ttu-id="0dd5a-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0dd5a-122">[identitySet][]</span></span>   | <span data-ttu-id="0dd5a-p104">Die Identität des Benutzers, des Geräts oder der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-p104">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="0dd5a-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0dd5a-125">createdDateTime</span></span>      | <span data-ttu-id="0dd5a-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dd5a-126">dateTimeOffset</span></span>    | <span data-ttu-id="0dd5a-p105">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-p105">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="0dd5a-129">eTag</span><span class="sxs-lookup"><span data-stu-id="0dd5a-129">eTag</span></span>                 | <span data-ttu-id="0dd5a-130">string</span><span class="sxs-lookup"><span data-stu-id="0dd5a-130">string</span></span>            | <span data-ttu-id="0dd5a-p106">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="0dd5a-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0dd5a-133">lastModifiedBy</span></span>       | <span data-ttu-id="0dd5a-134">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0dd5a-134">[identitySet][]</span></span>   | <span data-ttu-id="0dd5a-p107">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="0dd5a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0dd5a-137">lastModifiedDateTime</span></span> | <span data-ttu-id="0dd5a-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dd5a-138">dateTimeOffset</span></span>    | <span data-ttu-id="0dd5a-p108">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="0dd5a-141">name</span><span class="sxs-lookup"><span data-stu-id="0dd5a-141">name</span></span>                 | <span data-ttu-id="0dd5a-142">string</span><span class="sxs-lookup"><span data-stu-id="0dd5a-142">string</span></span>            | <span data-ttu-id="0dd5a-p109">Der Name des Elements. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="0dd5a-145">parentReference</span><span class="sxs-lookup"><span data-stu-id="0dd5a-145">parentReference</span></span>      | <span data-ttu-id="0dd5a-146">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="0dd5a-146">[itemReference][]</span></span> | <span data-ttu-id="0dd5a-p110">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="0dd5a-149">webUrl</span><span class="sxs-lookup"><span data-stu-id="0dd5a-149">webUrl</span></span>               | <span data-ttu-id="0dd5a-150">String (URL)</span><span class="sxs-lookup"><span data-stu-id="0dd5a-150">string (url)</span></span>      | <span data-ttu-id="0dd5a-p111">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="0dd5a-155">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="0dd5a-155">Remarks</span></span>

<span data-ttu-id="0dd5a-156">Der Typ `baseItem` wird voraussichtlich nicht direkt verwendet.</span><span class="sxs-lookup"><span data-stu-id="0dd5a-156">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
