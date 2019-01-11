---
title: Ressourcentyp attributeMapping
description: Definiert, wie die Werte für das angegebene Ziel-Attribut während der Synchronisation übertragen werden soll.
localization_priority: Normal
ms.openlocfilehash: 6c7a6367684b3e11013355b6d4726afe3346dab9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825277"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="5b3bd-103">Ressourcentyp attributeMapping</span><span class="sxs-lookup"><span data-stu-id="5b3bd-103">attributeMapping resource type</span></span>

> <span data-ttu-id="5b3bd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b3bd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b3bd-106">Definiert, wie die Werte für das angegebene Ziel-Attribut während der Synchronisation übertragen werden soll.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-106">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="5b3bd-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5b3bd-107">Properties</span></span>

| <span data-ttu-id="5b3bd-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5b3bd-108">Property</span></span>                  | <span data-ttu-id="5b3bd-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5b3bd-109">Type</span></span>                      | <span data-ttu-id="5b3bd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b3bd-110">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="5b3bd-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="5b3bd-111">defaultValue</span></span>               | <span data-ttu-id="5b3bd-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5b3bd-112">String</span></span>                    |<span data-ttu-id="5b3bd-113">Standardwert verwendet werden, für den Fall, dass die **Source** -Eigenschaft auf ausgewertet wurde `null`.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-113">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="5b3bd-114">Optional.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-114">Optional.</span></span>|
|<span data-ttu-id="5b3bd-115">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="5b3bd-115">exportMissingReferences</span></span>    |<span data-ttu-id="5b3bd-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5b3bd-116">String</span></span>                     |<span data-ttu-id="5b3bd-117">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-117">For internal use only.</span></span>|
|<span data-ttu-id="5b3bd-118">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="5b3bd-118">flowBehavior</span></span>               |<span data-ttu-id="5b3bd-119">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="5b3bd-119">attributeFlowBehavior</span></span>      |<span data-ttu-id="5b3bd-120">Definiert, wenn dieses Attribut in das Zielverzeichnis exportiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-120">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="5b3bd-121">Mögliche Werte sind: `FlowWhenChanged` und `FlowAlways`.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-121">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="5b3bd-122">Der Standardwert lautet `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-122">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="5b3bd-123">Wechselkurs des Flusstyps</span><span class="sxs-lookup"><span data-stu-id="5b3bd-123">flowType</span></span>                   |<span data-ttu-id="5b3bd-124">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="5b3bd-124">attributeFlowType</span></span>          |<span data-ttu-id="5b3bd-125">Definiert, wenn dieses Attribut in das Zielverzeichnis aktualisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-125">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="5b3bd-126">Mögliche Werte sind: `Always` (Standard), `ObjectAddOnly` (nur wenn neues Objekt erstellt wird), `MultiValueAddOnly` (nur wenn die Änderung neue Werte ein Attribut mit mehreren Werten hinzugefügt werden).</span><span class="sxs-lookup"><span data-stu-id="5b3bd-126">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="5b3bd-127">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="5b3bd-127">matchingPriority</span></span>           |<span data-ttu-id="5b3bd-128">Int32</span><span class="sxs-lookup"><span data-stu-id="5b3bd-128">Int32</span></span>                      |<span data-ttu-id="5b3bd-129">Wenn größer als 0, wird dieses Attribut zum Ausführen einer anfänglichen Übereinstimmung zwischen Quell- und Ziel-Verzeichnissen-Objekte verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-129">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="5b3bd-130">Das Synchronisierungsmodul versucht, das mithilfe des Attributs mit dem niedrigsten Wert von übereinstimmenden Priorität zuerst übereinstimmende Objekt zu suchen.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-130">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="5b3bd-131">Wenn nicht gefunden, wird das Attribut mit der nächsten übereinstimmenden Priorität verwendet werden und so weiter ein bis Übereinstimmung gefunden wurde oder keine weiteren übereinstimmenden Attribute bleiben.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-131">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="5b3bd-132">Als übereinstimmende Attribute sollte nur Attribute, die erwartet werden, damit eindeutige Werte wie e-Mails, die verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-132">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="5b3bd-133">source</span><span class="sxs-lookup"><span data-stu-id="5b3bd-133">source</span></span>                     |[<span data-ttu-id="5b3bd-134">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="5b3bd-134">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="5b3bd-135">Definiert, wie ein Wert sein sollte extrahiert haben (oder transformiert), aus dem Quellobjekt.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-135">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="5b3bd-136">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="5b3bd-136">targetAttributeName</span></span>        |<span data-ttu-id="5b3bd-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5b3bd-137">String</span></span>                     |<span data-ttu-id="5b3bd-138">Name des Attributs im Zielobjekt.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-138">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5b3bd-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5b3bd-139">JSON representation</span></span>

<span data-ttu-id="5b3bd-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5b3bd-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
