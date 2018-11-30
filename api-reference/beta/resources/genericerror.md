---
title: Allgemeiner Fehler Ressourcentyp
description: Ein allgemeiner Fehler.
ms.openlocfilehash: caf3fbb99ad521fd807138ab230f6a1b8ae7bb16
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058832"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="f8b6a-103">Allgemeiner Fehler Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f8b6a-103">genericError resource type</span></span>

> <span data-ttu-id="f8b6a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f8b6a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8b6a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8b6a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8b6a-106">Ein allgemeiner Fehler.</span><span class="sxs-lookup"><span data-stu-id="f8b6a-106">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="f8b6a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8b6a-107">Properties</span></span>

| <span data-ttu-id="f8b6a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8b6a-108">Property</span></span> | <span data-ttu-id="f8b6a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f8b6a-109">Type</span></span> | <span data-ttu-id="f8b6a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8b6a-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f8b6a-111">message</span><span class="sxs-lookup"><span data-stu-id="f8b6a-111">message</span></span> | <span data-ttu-id="f8b6a-112">String</span><span class="sxs-lookup"><span data-stu-id="f8b6a-112">String</span></span> | <span data-ttu-id="f8b6a-113">Die Fehlermeldung.</span><span class="sxs-lookup"><span data-stu-id="f8b6a-113">The error message.</span></span> |
| <span data-ttu-id="f8b6a-114">code</span><span class="sxs-lookup"><span data-stu-id="f8b6a-114">code</span></span> | <span data-ttu-id="f8b6a-115">String</span><span class="sxs-lookup"><span data-stu-id="f8b6a-115">String</span></span> | <span data-ttu-id="f8b6a-116">Der Fehlercode.</span><span class="sxs-lookup"><span data-stu-id="f8b6a-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f8b6a-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8b6a-117">JSON representation</span></span>

<span data-ttu-id="f8b6a-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8b6a-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```