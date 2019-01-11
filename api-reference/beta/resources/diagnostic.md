---
title: Diagnose Ressourcentyp
description: Informationen zu einer Fehlermeldung oder einer Warnung für eine OneNote-Operation.
localization_priority: Normal
ms.openlocfilehash: 28cdd1c07bab0494a69cfb7ce6a5284238e1ff19
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845990"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="a2026-103">Diagnose Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a2026-103">diagnostic resource type</span></span>

> <span data-ttu-id="a2026-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a2026-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2026-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a2026-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2026-106">Informationen zu einer Fehlermeldung oder einer Warnung für eine OneNote-Operation.</span><span class="sxs-lookup"><span data-stu-id="a2026-106">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2026-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a2026-107">JSON representation</span></span>

<span data-ttu-id="a2026-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a2026-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a><span data-ttu-id="a2026-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a2026-109">Properties</span></span>
| <span data-ttu-id="a2026-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a2026-110">Property</span></span>     | <span data-ttu-id="a2026-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a2026-111">Type</span></span>   |<span data-ttu-id="a2026-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2026-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2026-113">message</span><span class="sxs-lookup"><span data-stu-id="a2026-113">message</span></span>|<span data-ttu-id="a2026-114">String</span><span class="sxs-lookup"><span data-stu-id="a2026-114">String</span></span>|<span data-ttu-id="a2026-115">Die Nachricht, beschreibt die Bedingung, die den Fehler oder eine Warnung ausgelöst.</span><span class="sxs-lookup"><span data-stu-id="a2026-115">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="a2026-116">url</span><span class="sxs-lookup"><span data-stu-id="a2026-116">url</span></span>|<span data-ttu-id="a2026-117">String</span><span class="sxs-lookup"><span data-stu-id="a2026-117">String</span></span>|<span data-ttu-id="a2026-118">Die Verknüpfung mit der Dokumentation für dieses Problem.</span><span class="sxs-lookup"><span data-stu-id="a2026-118">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
