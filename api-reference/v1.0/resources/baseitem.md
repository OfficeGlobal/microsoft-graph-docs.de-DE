---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: daee18357e3f19f646a816070ca41a660f7b7ed3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810948"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="30f52-102">baseItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="30f52-102">BaseItem resource type</span></span>

<span data-ttu-id="30f52-p101">Die **baseItem**-Ressource ist eine abstrakte Ressource, die einen gemeinsamen Satz von Eigenschaften enthält, die auch von mehreren anderen Ressourcen verwendet werden. Folgende Ressourcen werden u. a. von abgeleitet **baseItem** abgeleitet:</span><span class="sxs-lookup"><span data-stu-id="30f52-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="30f52-105">Laufwerk</span><span class="sxs-lookup"><span data-stu-id="30f52-105">drive</span></span>](drive.md)
* [<span data-ttu-id="30f52-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="30f52-106">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="30f52-107">site</span><span class="sxs-lookup"><span data-stu-id="30f52-107">site</span></span>](site.md)
* [<span data-ttu-id="30f52-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="30f52-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="30f52-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="30f52-109">JSON representation</span></span>

<span data-ttu-id="30f52-110">Es folgt eine JSON-Darstellung einer **baseItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="30f52-110">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
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

## <a name="properties"></a><span data-ttu-id="30f52-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="30f52-111">Properties</span></span>

| <span data-ttu-id="30f52-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="30f52-112">Property</span></span>             | <span data-ttu-id="30f52-113">Typ</span><span class="sxs-lookup"><span data-stu-id="30f52-113">Type</span></span>              | <span data-ttu-id="30f52-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30f52-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="30f52-115">id</span><span class="sxs-lookup"><span data-stu-id="30f52-115">id</span></span>                   | <span data-ttu-id="30f52-116">string</span><span class="sxs-lookup"><span data-stu-id="30f52-116">string</span></span>            | <span data-ttu-id="30f52-p102">Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30f52-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="30f52-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="30f52-119">createdBy</span></span>            | <span data-ttu-id="30f52-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="30f52-120">[identitySet][]</span></span>   | <span data-ttu-id="30f52-p103">Die Identität des Benutzers, des Geräts oder der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30f52-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="30f52-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30f52-123">createdDateTime</span></span>      | <span data-ttu-id="30f52-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30f52-124">dateTimeOffset</span></span>    | <span data-ttu-id="30f52-p104">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30f52-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="30f52-127">description</span><span class="sxs-lookup"><span data-stu-id="30f52-127">description</span></span>          | <span data-ttu-id="30f52-128">String</span><span class="sxs-lookup"><span data-stu-id="30f52-128">String</span></span>            | <span data-ttu-id="30f52-129">Enthält eine Benutzer sichtbaren Beschreibung des Elements.</span><span class="sxs-lookup"><span data-stu-id="30f52-129">Provides a user-visible description of the item.</span></span> <span data-ttu-id="30f52-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="30f52-130">Optional.</span></span>                             |
| <span data-ttu-id="30f52-131">eTag</span><span class="sxs-lookup"><span data-stu-id="30f52-131">eTag</span></span>                 | <span data-ttu-id="30f52-132">string</span><span class="sxs-lookup"><span data-stu-id="30f52-132">string</span></span>            | <span data-ttu-id="30f52-p106">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30f52-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="30f52-135">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="30f52-135">lastModifiedBy</span></span>       | <span data-ttu-id="30f52-136">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="30f52-136">[identitySet][]</span></span>   | <span data-ttu-id="30f52-p107">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30f52-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="30f52-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30f52-139">lastModifiedDateTime</span></span> | <span data-ttu-id="30f52-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30f52-140">dateTimeOffset</span></span>    | <span data-ttu-id="30f52-p108">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30f52-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="30f52-143">name</span><span class="sxs-lookup"><span data-stu-id="30f52-143">name</span></span>                 | <span data-ttu-id="30f52-144">string</span><span class="sxs-lookup"><span data-stu-id="30f52-144">string</span></span>            | <span data-ttu-id="30f52-p109">Der Name des Elements. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="30f52-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="30f52-147">parentReference</span><span class="sxs-lookup"><span data-stu-id="30f52-147">parentReference</span></span>      | <span data-ttu-id="30f52-148">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="30f52-148">[itemReference][]</span></span> | <span data-ttu-id="30f52-p110">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="30f52-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="30f52-151">webUrl</span><span class="sxs-lookup"><span data-stu-id="30f52-151">webUrl</span></span>               | <span data-ttu-id="30f52-152">String (URL)</span><span class="sxs-lookup"><span data-stu-id="30f52-152">string (url)</span></span>      | <span data-ttu-id="30f52-p111">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30f52-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="30f52-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="30f52-155">Relationships</span></span>

| <span data-ttu-id="30f52-156">Beziehung</span><span class="sxs-lookup"><span data-stu-id="30f52-156">Relationship</span></span>       | <span data-ttu-id="30f52-157">Typ</span><span class="sxs-lookup"><span data-stu-id="30f52-157">Type</span></span>     | <span data-ttu-id="30f52-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30f52-158">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="30f52-159">createdByUser</span><span class="sxs-lookup"><span data-stu-id="30f52-159">createdByUser</span></span>      | <span data-ttu-id="30f52-160">[user][]</span><span class="sxs-lookup"><span data-stu-id="30f52-160">[user][]</span></span> | <span data-ttu-id="30f52-161">Der Name des Benutzers, der das Element erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="30f52-161">Identity of the user who created the item.</span></span> <span data-ttu-id="30f52-162">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30f52-162">Read-only.</span></span>
| <span data-ttu-id="30f52-163">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="30f52-163">lastModifiedByUser</span></span> | <span data-ttu-id="30f52-164">[user][]</span><span class="sxs-lookup"><span data-stu-id="30f52-164">[user][]</span></span> | <span data-ttu-id="30f52-165">Der Name des Benutzers, der das Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="30f52-165">Identity of the user who last modified the item.</span></span> <span data-ttu-id="30f52-166">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30f52-166">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[Benutzer]: user.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="30f52-170">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="30f52-170">Remarks</span></span>

<span data-ttu-id="30f52-171">Der Typ `baseItem` wird voraussichtlich nicht direkt verwendet.</span><span class="sxs-lookup"><span data-stu-id="30f52-171">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
