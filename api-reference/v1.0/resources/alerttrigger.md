---
title: Ressourcentyp alertTrigger
description: Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).
author: Preetikr
ms.openlocfilehash: f0888e6caf78d806909f818a8b72fb21320e7796
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341267"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="ce331-103">Ressourcentyp alertTrigger</span><span class="sxs-lookup"><span data-stu-id="ce331-103">alertTrigger resource type</span></span>

<span data-ttu-id="ce331-104">Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).</span><span class="sxs-lookup"><span data-stu-id="ce331-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="ce331-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ce331-105">Properties</span></span>

| <span data-ttu-id="ce331-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ce331-106">Property</span></span>   | <span data-ttu-id="ce331-107">Typ</span><span class="sxs-lookup"><span data-stu-id="ce331-107">Type</span></span>|<span data-ttu-id="ce331-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce331-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce331-109">name</span><span class="sxs-lookup"><span data-stu-id="ce331-109">name</span></span>|<span data-ttu-id="ce331-110">String</span><span class="sxs-lookup"><span data-stu-id="ce331-110">String</span></span>|<span data-ttu-id="ce331-111">Der Name der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="ce331-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="ce331-112">type</span><span class="sxs-lookup"><span data-stu-id="ce331-112">type</span></span>|<span data-ttu-id="ce331-113">String</span><span class="sxs-lookup"><span data-stu-id="ce331-113">String</span></span>|<span data-ttu-id="ce331-114">Typ der Eigenschaft im Schlüssel / Wert-Paar für Auslegung.</span><span class="sxs-lookup"><span data-stu-id="ce331-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="ce331-115">String, Boolean, beispielsweise usw.</span><span class="sxs-lookup"><span data-stu-id="ce331-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="ce331-116">Wert</span><span class="sxs-lookup"><span data-stu-id="ce331-116">value</span></span>|<span data-ttu-id="ce331-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce331-117">String</span></span>|<span data-ttu-id="ce331-118">Der Wert der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="ce331-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce331-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ce331-119">JSON representation</span></span>

<span data-ttu-id="ce331-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ce331-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="ce331-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce331-121">Example</span></span>

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