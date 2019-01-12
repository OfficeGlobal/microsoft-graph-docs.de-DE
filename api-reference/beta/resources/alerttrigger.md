---
title: Ressourcentyp alertTrigger
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 56034fb566f960ec858b86cdb4bcac86e5b9b47a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946427"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="6b384-104">Ressourcentyp alertTrigger</span><span class="sxs-lookup"><span data-stu-id="6b384-104">alertTrigger resource type</span></span>

 > <span data-ttu-id="6b384-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6b384-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b384-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b384-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b384-107">Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).</span><span class="sxs-lookup"><span data-stu-id="6b384-107">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="6b384-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6b384-108">Properties</span></span>

| <span data-ttu-id="6b384-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b384-109">Property</span></span>   | <span data-ttu-id="6b384-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6b384-110">Type</span></span>|<span data-ttu-id="6b384-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b384-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b384-112">name</span><span class="sxs-lookup"><span data-stu-id="6b384-112">name</span></span>|<span data-ttu-id="6b384-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b384-113">String</span></span>|<span data-ttu-id="6b384-114">Der Name der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="6b384-114">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="6b384-115">type</span><span class="sxs-lookup"><span data-stu-id="6b384-115">type</span></span>|<span data-ttu-id="6b384-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b384-116">String</span></span>|<span data-ttu-id="6b384-117">Typ der Eigenschaft im Schlüssel / Wert-Paar für Auslegung.</span><span class="sxs-lookup"><span data-stu-id="6b384-117">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="6b384-118">String, Boolean, beispielsweise usw.</span><span class="sxs-lookup"><span data-stu-id="6b384-118">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="6b384-119">Wert</span><span class="sxs-lookup"><span data-stu-id="6b384-119">value</span></span>|<span data-ttu-id="6b384-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b384-120">String</span></span>|<span data-ttu-id="6b384-121">Der Wert der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="6b384-121">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b384-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6b384-122">JSON representation</span></span>

<span data-ttu-id="6b384-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6b384-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="6b384-124">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b384-124">Example</span></span>

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
