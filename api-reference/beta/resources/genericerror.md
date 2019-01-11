---
title: Allgemeiner Fehler Ressourcentyp
description: Ein allgemeiner Fehler.
localization_priority: Normal
ms.openlocfilehash: 744266ef8ffb17c4af4168d6239e5a5a30561936
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823569"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="a8259-103">Allgemeiner Fehler Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a8259-103">genericError resource type</span></span>

> <span data-ttu-id="a8259-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a8259-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8259-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8259-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8259-106">Ein allgemeiner Fehler.</span><span class="sxs-lookup"><span data-stu-id="a8259-106">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="a8259-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a8259-107">Properties</span></span>

| <span data-ttu-id="a8259-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8259-108">Property</span></span> | <span data-ttu-id="a8259-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a8259-109">Type</span></span> | <span data-ttu-id="a8259-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8259-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="a8259-111">message</span><span class="sxs-lookup"><span data-stu-id="a8259-111">message</span></span> | <span data-ttu-id="a8259-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8259-112">String</span></span> | <span data-ttu-id="a8259-113">Die Fehlermeldung.</span><span class="sxs-lookup"><span data-stu-id="a8259-113">The error message.</span></span> |
| <span data-ttu-id="a8259-114">code</span><span class="sxs-lookup"><span data-stu-id="a8259-114">code</span></span> | <span data-ttu-id="a8259-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8259-115">String</span></span> | <span data-ttu-id="a8259-116">Der Fehlercode.</span><span class="sxs-lookup"><span data-stu-id="a8259-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a8259-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a8259-117">JSON representation</span></span>

<span data-ttu-id="a8259-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8259-118">Here is a JSON representation of the resource.</span></span>

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
