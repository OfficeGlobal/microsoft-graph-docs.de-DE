---
title: Ressourcentyp alertTrigger
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: e375538806f09f85539f7a03e31c8a1ae041afdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866647"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="344ce-104">Ressourcentyp alertTrigger</span><span class="sxs-lookup"><span data-stu-id="344ce-104">alertTrigger resource type</span></span>

 > <span data-ttu-id="344ce-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="344ce-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="344ce-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="344ce-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="344ce-107">Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).</span><span class="sxs-lookup"><span data-stu-id="344ce-107">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="344ce-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="344ce-108">Properties</span></span>

| <span data-ttu-id="344ce-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="344ce-109">Property</span></span>   | <span data-ttu-id="344ce-110">Typ</span><span class="sxs-lookup"><span data-stu-id="344ce-110">Type</span></span>|<span data-ttu-id="344ce-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="344ce-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="344ce-112">name</span><span class="sxs-lookup"><span data-stu-id="344ce-112">name</span></span>|<span data-ttu-id="344ce-113">String</span><span class="sxs-lookup"><span data-stu-id="344ce-113">String</span></span>|<span data-ttu-id="344ce-114">Der Name der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="344ce-114">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="344ce-115">type</span><span class="sxs-lookup"><span data-stu-id="344ce-115">type</span></span>|<span data-ttu-id="344ce-116">String</span><span class="sxs-lookup"><span data-stu-id="344ce-116">String</span></span>|<span data-ttu-id="344ce-117">Typ der Eigenschaft im Schlüssel / Wert-Paar für Auslegung.</span><span class="sxs-lookup"><span data-stu-id="344ce-117">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="344ce-118">String, Boolean, beispielsweise usw.</span><span class="sxs-lookup"><span data-stu-id="344ce-118">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="344ce-119">Wert</span><span class="sxs-lookup"><span data-stu-id="344ce-119">value</span></span>|<span data-ttu-id="344ce-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="344ce-120">String</span></span>|<span data-ttu-id="344ce-121">Der Wert der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="344ce-121">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="344ce-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="344ce-122">JSON representation</span></span>

<span data-ttu-id="344ce-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="344ce-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="344ce-124">Beispiel</span><span class="sxs-lookup"><span data-stu-id="344ce-124">Example</span></span>

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
