---
author: rgregg
ms.author: rgregg
ms.date: 09/14/2017
title: Identität
localization_priority: Normal
ms.openlocfilehash: c1cd28f4c2932e4196605c408470948e5b570894
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847586"
---
# <a name="identity-resource-type"></a><span data-ttu-id="8db33-102">Identität Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8db33-102">identity resource type</span></span>

> <span data-ttu-id="8db33-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8db33-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8db33-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8db33-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8db33-p102">Die **Identity**-Ressource stellt eine Identität von einem _Akteur_ dar. Ein Akteur kann z. B. ein Benutzer, Gerät oder eine Anwendung sein.</span><span class="sxs-lookup"><span data-stu-id="8db33-p102">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8db33-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8db33-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="8db33-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8db33-108">Properties</span></span>

| <span data-ttu-id="8db33-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8db33-109">Property</span></span>            | <span data-ttu-id="8db33-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8db33-110">Type</span></span>   | <span data-ttu-id="8db33-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8db33-111">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8db33-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8db33-112">displayName</span></span>         | <span data-ttu-id="8db33-113">String</span><span class="sxs-lookup"><span data-stu-id="8db33-113">String</span></span> | <span data-ttu-id="8db33-p103">Der Anzeigenamen der Identität. Beachten Sie, dass dieser möglicherweise nicht immer verfügbar oder auf dem neuesten Stand ist. Wenn sich z. B. der Anzeigename eines Benutzers ändert, zeigt die API möglicherweise den neuen Wert in einer zukünftigen Antwort an, aber für die dem Benutzer zugeordneten Elemente wird mit [delta](../api/driveitem-delta.md) nicht angezeigt, dass sie sich geändert haben.</span><span class="sxs-lookup"><span data-stu-id="8db33-p103">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="8db33-117">id</span><span class="sxs-lookup"><span data-stu-id="8db33-117">id</span></span>                  | <span data-ttu-id="8db33-118">String</span><span class="sxs-lookup"><span data-stu-id="8db33-118">String</span></span> | <span data-ttu-id="8db33-119">Eindeutiger Bezeichner für die Identität.</span><span class="sxs-lookup"><span data-stu-id="8db33-119">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="8db33-120">tenantId</span><span class="sxs-lookup"><span data-stu-id="8db33-120">tenantId</span></span>            | <span data-ttu-id="8db33-121">String</span><span class="sxs-lookup"><span data-stu-id="8db33-121">String</span></span> | <span data-ttu-id="8db33-122">Eindeutige Identität des Mandanten (optional).</span><span class="sxs-lookup"><span data-stu-id="8db33-122">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="8db33-123">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="8db33-123">Remarks</span></span>

<span data-ttu-id="8db33-p104">Unter gewissen Umständen steht der eindeutige Bezeichner für den Akteur möglicherweise nicht zur Verfügung. In diesem Fall die wird die Eigenschaft **DisplayName** für die Identität zurückgegeben werden, aber die **Id**-Eigenschaft ist aus der Ressource nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="8db33-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"
} -->
