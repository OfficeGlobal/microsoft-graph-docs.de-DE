---
title: Ressourcentyp resultInfo
description: Der Typ des ResultInfo.
author: VinodRavichandran
ms.openlocfilehash: db208ed214213ec906dac18b65140f010014fc6c
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380408"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="77538-103">Ressourcentyp resultInfo</span><span class="sxs-lookup"><span data-stu-id="77538-103">resultInfo resource type</span></span>

> <span data-ttu-id="77538-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="77538-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77538-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77538-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77538-106">Der Typ des ResultInfo.</span><span class="sxs-lookup"><span data-stu-id="77538-106">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="77538-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77538-107">Properties</span></span>

| <span data-ttu-id="77538-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77538-108">Property</span></span> | <span data-ttu-id="77538-109">Typ</span><span class="sxs-lookup"><span data-stu-id="77538-109">Type</span></span>   | <span data-ttu-id="77538-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77538-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="77538-111">code</span><span class="sxs-lookup"><span data-stu-id="77538-111">code</span></span>     | <span data-ttu-id="77538-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77538-112">String</span></span> | <span data-ttu-id="77538-113">Der Ergebniscode.</span><span class="sxs-lookup"><span data-stu-id="77538-113">The result code.</span></span>     |
| <span data-ttu-id="77538-114">message</span><span class="sxs-lookup"><span data-stu-id="77538-114">message</span></span>  | <span data-ttu-id="77538-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77538-115">String</span></span> | <span data-ttu-id="77538-116">Die Nachricht.</span><span class="sxs-lookup"><span data-stu-id="77538-116">The message.</span></span>         |
| <span data-ttu-id="77538-117">subCode</span><span class="sxs-lookup"><span data-stu-id="77538-117">subCode</span></span>  | <span data-ttu-id="77538-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77538-118">String</span></span> | <span data-ttu-id="77538-119">Der untergeordneten Ergebniscode.</span><span class="sxs-lookup"><span data-stu-id="77538-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="77538-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77538-120">JSON representation</span></span>

<span data-ttu-id="77538-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77538-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="77538-122">Beispiel-Fehlerergebnis</span><span class="sxs-lookup"><span data-stu-id="77538-122">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="77538-123">Beispiel generische Erfolg Ergebnis</span><span class="sxs-lookup"><span data-stu-id="77538-123">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="77538-124">Beispiel-Eintrag Erfolg Ergebnis</span><span class="sxs-lookup"><span data-stu-id="77538-124">Example Record Success result</span></span>

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
