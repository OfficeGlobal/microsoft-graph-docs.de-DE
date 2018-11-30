---
title: insightIdentity
description: " Ressourcentyp"
ms.openlocfilehash: e13d08eb111844896c96b02ab22c52d2f598ce58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062749"
---
# <a name="insightidentity"></a><span data-ttu-id="2d896-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="2d896-103">insightIdentity</span></span>

> <span data-ttu-id="2d896-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2d896-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d896-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d896-105">Use of these APIs in production applications is not supported.</span></span>

 <span data-ttu-id="2d896-106">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2d896-106">resource type</span></span>

<span data-ttu-id="2d896-107">Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält.</span><span class="sxs-lookup"><span data-stu-id="2d896-107">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="2d896-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2d896-108">JSON representation</span></span>
<span data-ttu-id="2d896-109">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2d896-109">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="2d896-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2d896-110">Properties</span></span>

| <span data-ttu-id="2d896-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d896-111">Property</span></span>              | <span data-ttu-id="2d896-112">Typ</span><span class="sxs-lookup"><span data-stu-id="2d896-112">Type</span></span>          | <span data-ttu-id="2d896-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d896-113">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="2d896-114">displayName</span><span class="sxs-lookup"><span data-stu-id="2d896-114">displayName</span></span>       | <span data-ttu-id="2d896-115">String</span><span class="sxs-lookup"><span data-stu-id="2d896-115">String</span></span>          | <span data-ttu-id="2d896-116">Der Anzeigename des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="2d896-116">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="2d896-117">id</span><span class="sxs-lookup"><span data-stu-id="2d896-117">id</span></span>              | <span data-ttu-id="2d896-118">String</span><span class="sxs-lookup"><span data-stu-id="2d896-118">String</span></span>        | <span data-ttu-id="2d896-119">Die Id des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="2d896-119">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="2d896-120">address</span><span class="sxs-lookup"><span data-stu-id="2d896-120">address</span></span>             | <span data-ttu-id="2d896-121">String</span><span class="sxs-lookup"><span data-stu-id="2d896-121">String</span></span>      | <span data-ttu-id="2d896-122">Die e-Mail-Adresse des Benutzers, der das Element freigegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="2d896-122">The email address of the user who shared the item.</span></span>  |