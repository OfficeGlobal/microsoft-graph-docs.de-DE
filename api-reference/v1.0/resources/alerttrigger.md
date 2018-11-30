---
title: Ressourcentyp alertTrigger
description: Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).
ms.openlocfilehash: b4af3be67669fd27f27e888cbc28b60b0c1c67a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019345"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="e9e6e-103">Ressourcentyp alertTrigger</span><span class="sxs-lookup"><span data-stu-id="e9e6e-103">alertTrigger resource type</span></span>

<span data-ttu-id="e9e6e-104">Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).</span><span class="sxs-lookup"><span data-stu-id="e9e6e-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="e9e6e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e9e6e-105">Properties</span></span>

| <span data-ttu-id="e9e6e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e9e6e-106">Property</span></span>   | <span data-ttu-id="e9e6e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="e9e6e-107">Type</span></span>|<span data-ttu-id="e9e6e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9e6e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9e6e-109">name</span><span class="sxs-lookup"><span data-stu-id="e9e6e-109">name</span></span>|<span data-ttu-id="e9e6e-110">String</span><span class="sxs-lookup"><span data-stu-id="e9e6e-110">String</span></span>|<span data-ttu-id="e9e6e-111">Der Name der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="e9e6e-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="e9e6e-112">Typ</span><span class="sxs-lookup"><span data-stu-id="e9e6e-112">type</span></span>|<span data-ttu-id="e9e6e-113">String</span><span class="sxs-lookup"><span data-stu-id="e9e6e-113">String</span></span>|<span data-ttu-id="e9e6e-114">Typ der Eigenschaft im Schlüssel / Wert-Paar für Auslegung.</span><span class="sxs-lookup"><span data-stu-id="e9e6e-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="e9e6e-115">String, Boolean, beispielsweise usw.</span><span class="sxs-lookup"><span data-stu-id="e9e6e-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="e9e6e-116">Wert</span><span class="sxs-lookup"><span data-stu-id="e9e6e-116">value</span></span>|<span data-ttu-id="e9e6e-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e9e6e-117">String</span></span>|<span data-ttu-id="e9e6e-118">Der Wert der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="e9e6e-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9e6e-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e9e6e-119">JSON representation</span></span>

<span data-ttu-id="e9e6e-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e9e6e-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="e9e6e-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e9e6e-121">Example</span></span>

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