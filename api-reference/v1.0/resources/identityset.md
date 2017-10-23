---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
ms.openlocfilehash: 4d2bb5d92ebe06e79a68d69b949baec19a33a4c6
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="identityset-resource-type"></a><span data-ttu-id="ba0c7-102">IdentitySet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ba0c7-102">IdentitySet resource type</span></span>

<span data-ttu-id="ba0c7-p101">Die **IdentitySet**-Ressource ist eine verschlüsselte Sammlung von [identity](identity.md)-Ressourcen. Sie wird verwendet, um eine Reihe von Identitäten darzustellen, die verschiedenen Ereignissen für ein Element zugewiesen sind, z. B. _erstellt von_ oder _zuletzt geändert von_.</span><span class="sxs-lookup"><span data-stu-id="ba0c7-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba0c7-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ba0c7-105">JSON representation</span></span>

<span data-ttu-id="ba0c7-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ba0c7-106">Here is a JSON representation of the resource.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identitySet",
       "optionalProperties": ["user", "application", "device"],
       "openType": true } -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="ba0c7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ba0c7-107">Properties</span></span>

| <span data-ttu-id="ba0c7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ba0c7-108">Property</span></span>    | <span data-ttu-id="ba0c7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ba0c7-109">Type</span></span>                    | <span data-ttu-id="ba0c7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba0c7-110">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="ba0c7-111">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba0c7-111">application</span></span> | [<span data-ttu-id="ba0c7-112">Identity</span><span class="sxs-lookup"><span data-stu-id="ba0c7-112">Identity</span></span>](identity.md) | <span data-ttu-id="ba0c7-p102">Optional. Die mit dieser Aktion verknüpfte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="ba0c7-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="ba0c7-115">Gerät</span><span class="sxs-lookup"><span data-stu-id="ba0c7-115">device</span></span>      | [<span data-ttu-id="ba0c7-116">Identity</span><span class="sxs-lookup"><span data-stu-id="ba0c7-116">Identity</span></span>](identity.md) | <span data-ttu-id="ba0c7-p103">Optional. Das mit dieser Konfiguration verknüpfte Gerät.</span><span class="sxs-lookup"><span data-stu-id="ba0c7-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="ba0c7-119">Benutzer</span><span class="sxs-lookup"><span data-stu-id="ba0c7-119">user</span></span>        | [<span data-ttu-id="ba0c7-120">Identity</span><span class="sxs-lookup"><span data-stu-id="ba0c7-120">Identity</span></span>](identity.md) | <span data-ttu-id="ba0c7-p104">Optional. Der mit dieser Aktion verknüpfte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="ba0c7-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="ba0c7-123">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="ba0c7-123">Remarks</span></span> 

<span data-ttu-id="ba0c7-124">Informationen zur Verwendung von [IdentitySet](driveitem.md)-Ressourcen finden Sie unter **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="ba0c7-124">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
