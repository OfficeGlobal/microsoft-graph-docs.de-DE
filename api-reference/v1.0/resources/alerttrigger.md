---
title: Ressourcentyp alertTrigger
description: Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).
author: Preetikr
localization_priority: Normal
ms.openlocfilehash: 1dc8bb2b18380da50134aa67e742da89dea3c057
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894341"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="0623d-103">Ressourcentyp alertTrigger</span><span class="sxs-lookup"><span data-stu-id="0623d-103">alertTrigger resource type</span></span>

<span data-ttu-id="0623d-104">Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).</span><span class="sxs-lookup"><span data-stu-id="0623d-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="0623d-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0623d-105">Properties</span></span>

| <span data-ttu-id="0623d-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0623d-106">Property</span></span>   | <span data-ttu-id="0623d-107">Typ</span><span class="sxs-lookup"><span data-stu-id="0623d-107">Type</span></span>|<span data-ttu-id="0623d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0623d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0623d-109">name</span><span class="sxs-lookup"><span data-stu-id="0623d-109">name</span></span>|<span data-ttu-id="0623d-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0623d-110">String</span></span>|<span data-ttu-id="0623d-111">Der Name der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="0623d-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="0623d-112">type</span><span class="sxs-lookup"><span data-stu-id="0623d-112">type</span></span>|<span data-ttu-id="0623d-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0623d-113">String</span></span>|<span data-ttu-id="0623d-114">Typ der Eigenschaft im Schlüssel / Wert-Paar für Auslegung.</span><span class="sxs-lookup"><span data-stu-id="0623d-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="0623d-115">String, Boolean, beispielsweise usw.</span><span class="sxs-lookup"><span data-stu-id="0623d-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="0623d-116">Wert</span><span class="sxs-lookup"><span data-stu-id="0623d-116">value</span></span>|<span data-ttu-id="0623d-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0623d-117">String</span></span>|<span data-ttu-id="0623d-118">Der Wert der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="0623d-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0623d-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0623d-119">JSON representation</span></span>

<span data-ttu-id="0623d-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0623d-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="0623d-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0623d-121">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
