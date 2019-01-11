---
title: Ressourcentyp resultInfo
description: Der Typ des ResultInfo.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: ca814fd5c44f0f811099faed53354d08ce8befdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855279"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="077b9-103">Ressourcentyp resultInfo</span><span class="sxs-lookup"><span data-stu-id="077b9-103">resultInfo resource type</span></span>

> <span data-ttu-id="077b9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="077b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="077b9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="077b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="077b9-106">Der Typ des ResultInfo.</span><span class="sxs-lookup"><span data-stu-id="077b9-106">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="077b9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="077b9-107">Properties</span></span>

| <span data-ttu-id="077b9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="077b9-108">Property</span></span> | <span data-ttu-id="077b9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="077b9-109">Type</span></span>   | <span data-ttu-id="077b9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="077b9-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="077b9-111">code</span><span class="sxs-lookup"><span data-stu-id="077b9-111">code</span></span>     | <span data-ttu-id="077b9-112">String</span><span class="sxs-lookup"><span data-stu-id="077b9-112">String</span></span> | <span data-ttu-id="077b9-113">Der Ergebniscode.</span><span class="sxs-lookup"><span data-stu-id="077b9-113">The result code.</span></span>     |
| <span data-ttu-id="077b9-114">message</span><span class="sxs-lookup"><span data-stu-id="077b9-114">message</span></span>  | <span data-ttu-id="077b9-115">String</span><span class="sxs-lookup"><span data-stu-id="077b9-115">String</span></span> | <span data-ttu-id="077b9-116">Die Nachricht.</span><span class="sxs-lookup"><span data-stu-id="077b9-116">The message.</span></span>         |
| <span data-ttu-id="077b9-117">subCode</span><span class="sxs-lookup"><span data-stu-id="077b9-117">subCode</span></span>  | <span data-ttu-id="077b9-118">String</span><span class="sxs-lookup"><span data-stu-id="077b9-118">String</span></span> | <span data-ttu-id="077b9-119">Der untergeordneten Ergebniscode.</span><span class="sxs-lookup"><span data-stu-id="077b9-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="077b9-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="077b9-120">JSON representation</span></span>

<span data-ttu-id="077b9-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="077b9-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "String",
  "message": "String",
  "subCode": "String"
}
```

## <a name="example-error-result"></a><span data-ttu-id="077b9-122">Beispiel-Fehlerergebnis</span><span class="sxs-lookup"><span data-stu-id="077b9-122">Example Error result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "100",
  "message": "Internal Server Error.",
  "subCode": "20"
}
```

## <a name="example-generic-success-result"></a><span data-ttu-id="077b9-123">Beispiel generische Erfolg Ergebnis</span><span class="sxs-lookup"><span data-stu-id="077b9-123">Example Generic success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "0"
}
```

## <a name="example-record-success-result"></a><span data-ttu-id="077b9-124">Beispiel-Eintrag Erfolg Ergebnis</span><span class="sxs-lookup"><span data-stu-id="077b9-124">Example Record Success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "completedSilenceDetected"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
