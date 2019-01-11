---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: 63178fc9add3d097b7e8aaf0c5c2a697a91eaeed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807021"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="b63b5-102">Ressourcentyp identitySet</span><span class="sxs-lookup"><span data-stu-id="b63b5-102">identitySet resource type</span></span>

<span data-ttu-id="b63b5-p101">Die **IdentitySet**-Ressource ist eine verschlüsselte Sammlung von [identity](identity.md)-Ressourcen. Sie wird verwendet, um eine Reihe von Identitäten darzustellen, die verschiedenen Ereignissen für ein Element zugewiesen sind, z. B. _erstellt von_ oder _zuletzt geändert von_.</span><span class="sxs-lookup"><span data-stu-id="b63b5-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b63b5-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b63b5-105">JSON representation</span></span>

<span data-ttu-id="b63b5-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b63b5-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "device",
    "encrypted",
    "guest",
    "phone",
    "user"
  ],
  "openType": true
} -->
```json
{
  "application": {"@odata.type": "#microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "#microsoft.graph.identity"},
  "device": {"@odata.type": "#microsoft.graph.identity"},
  "encrypted": {"@odata.type": "#microsoft.graph.identity"},
  "guest": {"@odata.type": "#microsoft.graph.identity"},
  "phone": {"@odata.type": "#microsoft.graph.identity"},
  "user": {"@odata.type": "#microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="b63b5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b63b5-107">Properties</span></span>

| <span data-ttu-id="b63b5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b63b5-108">Property</span></span>    | <span data-ttu-id="b63b5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b63b5-109">Type</span></span>                    | <span data-ttu-id="b63b5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b63b5-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="b63b5-111">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b63b5-111">application</span></span> | [<span data-ttu-id="b63b5-112">Identity</span><span class="sxs-lookup"><span data-stu-id="b63b5-112">Identity</span></span>](identity.md) | <span data-ttu-id="b63b5-p102">Optional. Die mit dieser Aktion verknüpfte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="b63b5-p102">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="b63b5-115">Gerät</span><span class="sxs-lookup"><span data-stu-id="b63b5-115">device</span></span>      | [<span data-ttu-id="b63b5-116">Identity</span><span class="sxs-lookup"><span data-stu-id="b63b5-116">Identity</span></span>](identity.md) | <span data-ttu-id="b63b5-p103">Optional. Das mit dieser Konfiguration verknüpfte Gerät.</span><span class="sxs-lookup"><span data-stu-id="b63b5-p103">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="b63b5-119">phone</span><span class="sxs-lookup"><span data-stu-id="b63b5-119">phone</span></span>       | [<span data-ttu-id="b63b5-120">identity</span><span class="sxs-lookup"><span data-stu-id="b63b5-120">identity</span></span>](identity.md) | <span data-ttu-id="b63b5-121">Optional.</span><span class="sxs-lookup"><span data-stu-id="b63b5-121">Optional.</span></span> <span data-ttu-id="b63b5-122">Die Telefonnummer, die diese Aktion zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="b63b5-122">The phone number associated with this action.</span></span> |
| <span data-ttu-id="b63b5-123">Benutzer</span><span class="sxs-lookup"><span data-stu-id="b63b5-123">user</span></span>        | [<span data-ttu-id="b63b5-124">Identity</span><span class="sxs-lookup"><span data-stu-id="b63b5-124">Identity</span></span>](identity.md) | <span data-ttu-id="b63b5-p105">Optional. Der mit dieser Aktion verknüpfte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="b63b5-p105">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="b63b5-127">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="b63b5-127">Remarks</span></span> 

<span data-ttu-id="b63b5-128">Verwendung der **IdentitySet** Ressourcen finden Sie unter [aufrufen](call.md) .</span><span class="sxs-lookup"><span data-stu-id="b63b5-128">See [Call](call.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
