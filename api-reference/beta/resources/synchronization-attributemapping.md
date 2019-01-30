---
title: Ressourcentyp attributeMapping
description: Definiert, wie die Werte für das angegebene Ziel-Attribut während der Synchronisation übertragen werden soll.
localization_priority: Normal
ms.openlocfilehash: 16235cce73a17b462f6f44aedf0c8759277983c1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641876"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="47e90-103">Ressourcentyp attributeMapping</span><span class="sxs-lookup"><span data-stu-id="47e90-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47e90-104">Definiert, wie die Werte für das angegebene Ziel-Attribut während der Synchronisation übertragen werden soll.</span><span class="sxs-lookup"><span data-stu-id="47e90-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="47e90-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="47e90-105">Properties</span></span>

| <span data-ttu-id="47e90-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="47e90-106">Property</span></span>                  | <span data-ttu-id="47e90-107">Typ</span><span class="sxs-lookup"><span data-stu-id="47e90-107">Type</span></span>                      | <span data-ttu-id="47e90-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47e90-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="47e90-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="47e90-109">defaultValue</span></span>               | <span data-ttu-id="47e90-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="47e90-110">String</span></span>                    |<span data-ttu-id="47e90-111">Standardwert verwendet werden, für den Fall, dass die **Source** -Eigenschaft auf ausgewertet wurde `null`.</span><span class="sxs-lookup"><span data-stu-id="47e90-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="47e90-112">Optional.</span><span class="sxs-lookup"><span data-stu-id="47e90-112">Optional.</span></span>|
|<span data-ttu-id="47e90-113">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="47e90-113">exportMissingReferences</span></span>    |<span data-ttu-id="47e90-114">String</span><span class="sxs-lookup"><span data-stu-id="47e90-114">String</span></span>                     |<span data-ttu-id="47e90-115">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="47e90-115">For internal use only.</span></span>|
|<span data-ttu-id="47e90-116">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="47e90-116">flowBehavior</span></span>               |<span data-ttu-id="47e90-117">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="47e90-117">attributeFlowBehavior</span></span>      |<span data-ttu-id="47e90-118">Definiert, wenn dieses Attribut in das Zielverzeichnis exportiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="47e90-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="47e90-119">Mögliche Werte sind: `FlowWhenChanged` und `FlowAlways`.</span><span class="sxs-lookup"><span data-stu-id="47e90-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="47e90-120">Der Standardwert lautet `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="47e90-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="47e90-121">Wechselkurs des Flusstyps</span><span class="sxs-lookup"><span data-stu-id="47e90-121">flowType</span></span>                   |<span data-ttu-id="47e90-122">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="47e90-122">attributeFlowType</span></span>          |<span data-ttu-id="47e90-123">Definiert, wenn dieses Attribut in das Zielverzeichnis aktualisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="47e90-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="47e90-124">Mögliche Werte sind: `Always` (Standard), `ObjectAddOnly` (nur wenn neues Objekt erstellt wird), `MultiValueAddOnly` (nur wenn die Änderung neue Werte ein Attribut mit mehreren Werten hinzugefügt werden).</span><span class="sxs-lookup"><span data-stu-id="47e90-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="47e90-125">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="47e90-125">matchingPriority</span></span>           |<span data-ttu-id="47e90-126">Int32</span><span class="sxs-lookup"><span data-stu-id="47e90-126">Int32</span></span>                      |<span data-ttu-id="47e90-127">Wenn größer als 0, wird dieses Attribut zum Ausführen einer anfänglichen Übereinstimmung zwischen Quell- und Ziel-Verzeichnissen-Objekte verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="47e90-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="47e90-128">Das Synchronisierungsmodul versucht, das mithilfe des Attributs mit dem niedrigsten Wert von übereinstimmenden Priorität zuerst übereinstimmende Objekt zu suchen.</span><span class="sxs-lookup"><span data-stu-id="47e90-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="47e90-129">Wenn nicht gefunden, wird das Attribut mit der nächsten übereinstimmenden Priorität verwendet werden und so weiter ein bis Übereinstimmung gefunden wurde oder keine weiteren übereinstimmenden Attribute bleiben.</span><span class="sxs-lookup"><span data-stu-id="47e90-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="47e90-130">Als übereinstimmende Attribute sollte nur Attribute, die erwartet werden, damit eindeutige Werte wie e-Mails, die verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="47e90-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="47e90-131">source</span><span class="sxs-lookup"><span data-stu-id="47e90-131">source</span></span>                     |[<span data-ttu-id="47e90-132">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="47e90-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="47e90-133">Definiert, wie ein Wert sein sollte extrahiert haben (oder transformiert), aus dem Quellobjekt.</span><span class="sxs-lookup"><span data-stu-id="47e90-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="47e90-134">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="47e90-134">targetAttributeName</span></span>        |<span data-ttu-id="47e90-135">String</span><span class="sxs-lookup"><span data-stu-id="47e90-135">String</span></span>                     |<span data-ttu-id="47e90-136">Name des Attributs im Zielobjekt.</span><span class="sxs-lookup"><span data-stu-id="47e90-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="47e90-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="47e90-137">JSON representation</span></span>

<span data-ttu-id="47e90-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="47e90-138">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
