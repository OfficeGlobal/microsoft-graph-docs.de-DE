---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: 0a963f7158dbb812fc1f51fbff208297a2a9f076
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482196"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="d831a-102">identityset-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d831a-102">identitySet resource type</span></span>

<span data-ttu-id="d831a-p101">Die **IdentitySet**-Ressource ist eine verschlüsselte Sammlung von [identity](identity.md)-Ressourcen. Sie wird verwendet, um eine Reihe von Identitäten darzustellen, die verschiedenen Ereignissen für ein Element zugewiesen sind, z. B. _erstellt von_ oder _zuletzt geändert von_.</span><span class="sxs-lookup"><span data-stu-id="d831a-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d831a-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d831a-105">JSON representation</span></span>

<span data-ttu-id="d831a-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d831a-106">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d831a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d831a-107">Properties</span></span>

| <span data-ttu-id="d831a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d831a-108">Property</span></span>    | <span data-ttu-id="d831a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d831a-109">Type</span></span>                    | <span data-ttu-id="d831a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d831a-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="d831a-111">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d831a-111">application</span></span> | [<span data-ttu-id="d831a-112">Identity</span><span class="sxs-lookup"><span data-stu-id="d831a-112">Identity</span></span>](identity.md) | <span data-ttu-id="d831a-p102">Optional. Die mit dieser Aktion verknüpfte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="d831a-p102">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="d831a-115">Gerät</span><span class="sxs-lookup"><span data-stu-id="d831a-115">device</span></span>      | [<span data-ttu-id="d831a-116">Identity</span><span class="sxs-lookup"><span data-stu-id="d831a-116">Identity</span></span>](identity.md) | <span data-ttu-id="d831a-p103">Optional. Das mit dieser Konfiguration verknüpfte Gerät.</span><span class="sxs-lookup"><span data-stu-id="d831a-p103">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="d831a-119">phone</span><span class="sxs-lookup"><span data-stu-id="d831a-119">phone</span></span>       | [<span data-ttu-id="d831a-120">identity</span><span class="sxs-lookup"><span data-stu-id="d831a-120">identity</span></span>](identity.md) | <span data-ttu-id="d831a-121">Optional.</span><span class="sxs-lookup"><span data-stu-id="d831a-121">Optional.</span></span> <span data-ttu-id="d831a-122">Die Telefonnummer, die dieser Aktion zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="d831a-122">The phone number associated with this action.</span></span> |
| <span data-ttu-id="d831a-123">Benutzer</span><span class="sxs-lookup"><span data-stu-id="d831a-123">user</span></span>        | [<span data-ttu-id="d831a-124">Identity</span><span class="sxs-lookup"><span data-stu-id="d831a-124">Identity</span></span>](identity.md) | <span data-ttu-id="d831a-p105">Optional. Der mit dieser Aktion verknüpfte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="d831a-p105">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="d831a-127">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="d831a-127">Remarks</span></span> 

<span data-ttu-id="d831a-128">Weitere Informationen finden Sie unter [Aufruf](call.md) zur Verwendung von **identityset** -Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="d831a-128">See [Call](call.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
