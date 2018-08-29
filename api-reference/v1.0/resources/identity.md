---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Identität
ms.openlocfilehash: 521952ab8ea3350fcf29aa80cb82928e5017e5bb
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267164"
---
# <a name="identity-resource-type"></a><span data-ttu-id="57b79-102">identity-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="57b79-102">Identity resource type</span></span>

<span data-ttu-id="57b79-p101">Die **Identity**-Ressource stellt eine Identität von einem _Akteur_ dar. Ein Akteur kann z. B. ein Benutzer, Gerät oder eine Anwendung sein.</span><span class="sxs-lookup"><span data-stu-id="57b79-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="57b79-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="57b79-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity",
  "openType": true,
 "optionalProperties": ["displayName", "thumbnails"] } -->
```json
{
  "displayName": "string",
  "id": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="57b79-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="57b79-106">Properties</span></span>

| <span data-ttu-id="57b79-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="57b79-107">Property</span></span>    | <span data-ttu-id="57b79-108">Typ</span><span class="sxs-lookup"><span data-stu-id="57b79-108">Type</span></span>   | <span data-ttu-id="57b79-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57b79-109">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="57b79-110">displayName</span><span class="sxs-lookup"><span data-stu-id="57b79-110">displayName</span></span> | <span data-ttu-id="57b79-111">String</span><span class="sxs-lookup"><span data-stu-id="57b79-111">String</span></span> | <span data-ttu-id="57b79-p102">Der Anzeigenamen der Identität. Beachten Sie, dass dieser möglicherweise nicht immer verfügbar oder auf dem neuesten Stand ist. Wenn sich z. B. der Anzeigename eines Benutzers ändert, zeigt die API möglicherweise den neuen Wert in einer zukünftigen Antwort an, aber für die dem Benutzer zugeordneten Elemente wird mit [delta](../api/driveitem_delta.md) nicht angezeigt, dass sie sich geändert haben.</span><span class="sxs-lookup"><span data-stu-id="57b79-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem_delta.md).</span></span>     |
| <span data-ttu-id="57b79-115">id</span><span class="sxs-lookup"><span data-stu-id="57b79-115">id</span></span>          | <span data-ttu-id="57b79-116">String</span><span class="sxs-lookup"><span data-stu-id="57b79-116">String</span></span> | <span data-ttu-id="57b79-117">Eindeutiger Bezeichner für die Identität.</span><span class="sxs-lookup"><span data-stu-id="57b79-117">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |

## <a name="remarks"></a><span data-ttu-id="57b79-118">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="57b79-118">Remarks</span></span>

<span data-ttu-id="57b79-p103">Unter gewissen Umständen steht der eindeutige Bezeichner für den Akteur möglicherweise nicht zur Verfügung. In diesem Fall die wird die Eigenschaft **DisplayName** für die Identität zurückgegeben werden, aber die **Id**-Eigenschaft ist aus der Ressource nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="57b79-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"

} -->
