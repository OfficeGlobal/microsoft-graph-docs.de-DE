---
title: insightIdentity
description: Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 395c865a38ebe6ea84dc64857f441cd529e4f2d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886576"
---
# <a name="insightidentity"></a><span data-ttu-id="03be6-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="03be6-103">insightIdentity</span></span>

> <span data-ttu-id="03be6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="03be6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03be6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="03be6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03be6-106">Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält.</span><span class="sxs-lookup"><span data-stu-id="03be6-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="03be6-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="03be6-107">JSON representation</span></span>
<span data-ttu-id="03be6-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="03be6-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="03be6-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="03be6-109">Properties</span></span>

| <span data-ttu-id="03be6-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03be6-110">Property</span></span>              | <span data-ttu-id="03be6-111">Typ</span><span class="sxs-lookup"><span data-stu-id="03be6-111">Type</span></span>          | <span data-ttu-id="03be6-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03be6-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="03be6-113">displayName</span><span class="sxs-lookup"><span data-stu-id="03be6-113">displayName</span></span>       | <span data-ttu-id="03be6-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="03be6-114">String</span></span>          | <span data-ttu-id="03be6-115">Der Anzeigename des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="03be6-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="03be6-116">id</span><span class="sxs-lookup"><span data-stu-id="03be6-116">id</span></span>              | <span data-ttu-id="03be6-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="03be6-117">String</span></span>        | <span data-ttu-id="03be6-118">Die Id des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="03be6-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="03be6-119">address</span><span class="sxs-lookup"><span data-stu-id="03be6-119">address</span></span>             | <span data-ttu-id="03be6-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="03be6-120">String</span></span>      | <span data-ttu-id="03be6-121">Die e-Mail-Adresse des Benutzers, der das Element freigegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="03be6-121">The email address of the user who shared the item.</span></span>  |
