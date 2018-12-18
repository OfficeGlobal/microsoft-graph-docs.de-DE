---
title: insightIdentity
description: Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält.
author: simonhult
ms.openlocfilehash: 648242b827c0390029522955b0fe6347b98100c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331332"
---
# <a name="insightidentity"></a><span data-ttu-id="e5d5c-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="e5d5c-103">insightIdentity</span></span>

> <span data-ttu-id="e5d5c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e5d5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5d5c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5d5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5d5c-106">Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält.</span><span class="sxs-lookup"><span data-stu-id="e5d5c-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="e5d5c-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e5d5c-107">JSON representation</span></span>
<span data-ttu-id="e5d5c-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e5d5c-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="e5d5c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e5d5c-109">Properties</span></span>

| <span data-ttu-id="e5d5c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e5d5c-110">Property</span></span>              | <span data-ttu-id="e5d5c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e5d5c-111">Type</span></span>          | <span data-ttu-id="e5d5c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5d5c-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="e5d5c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="e5d5c-113">displayName</span></span>       | <span data-ttu-id="e5d5c-114">String</span><span class="sxs-lookup"><span data-stu-id="e5d5c-114">String</span></span>          | <span data-ttu-id="e5d5c-115">Der Anzeigename des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="e5d5c-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="e5d5c-116">id</span><span class="sxs-lookup"><span data-stu-id="e5d5c-116">id</span></span>              | <span data-ttu-id="e5d5c-117">String</span><span class="sxs-lookup"><span data-stu-id="e5d5c-117">String</span></span>        | <span data-ttu-id="e5d5c-118">Die Id des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="e5d5c-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="e5d5c-119">address</span><span class="sxs-lookup"><span data-stu-id="e5d5c-119">address</span></span>             | <span data-ttu-id="e5d5c-120">String</span><span class="sxs-lookup"><span data-stu-id="e5d5c-120">String</span></span>      | <span data-ttu-id="e5d5c-121">Die e-Mail-Adresse des Benutzers, der das Element freigegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="e5d5c-121">The email address of the user who shared the item.</span></span>  |