---
title: singleValueLegacyExtendedProperty-Ressourcentyp
description: 'Eine erweiterte Eigenschaft, die einen einzelnen Wert enthält. '
localization_priority: Normal
ms.openlocfilehash: f865da1a8a4211ac99a70881b2851b38b8e72727
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894229"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="9fb8a-103">singleValueLegacyExtendedProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9fb8a-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="9fb8a-104">Eine erweiterte Eigenschaft, die einen einzelnen Wert enthält.</span><span class="sxs-lookup"><span data-stu-id="9fb8a-104">An extended property that contains a single value.</span></span> 

<span data-ttu-id="9fb8a-105">Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="9fb8a-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="9fb8a-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="9fb8a-106">Methods</span></span>

| <span data-ttu-id="9fb8a-107">Methode</span><span class="sxs-lookup"><span data-stu-id="9fb8a-107">Method</span></span>           | <span data-ttu-id="9fb8a-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9fb8a-108">Return Type</span></span>    |<span data-ttu-id="9fb8a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fb8a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9fb8a-110">Post</span><span class="sxs-lookup"><span data-stu-id="9fb8a-110">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="9fb8a-111">Eine unterstützte Ressourceninstanz: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) oder [contactFolder](../resources/contactfolder.md), aber nicht [post](../resources/post.md) für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="9fb8a-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="9fb8a-112">Erstellen einer **singleValueLegacyExtendedProperty** in einer neuen oder vorhandenen Instanz einer unterstützten Ressource.</span><span class="sxs-lookup"><span data-stu-id="9fb8a-112">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="9fb8a-113">Get</span><span class="sxs-lookup"><span data-stu-id="9fb8a-113">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="9fb8a-114">Eine unterstützte Ressourceninstanz oder eine Sammlung von unterstützten Ressourceninstanzen ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) oder [post](../resources/post.md) für die Gruppe) oder eine solche Instanz erweitert mit einem [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="9fb8a-114">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="9fb8a-115">Abrufen einer Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="9fb8a-115">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="9fb8a-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9fb8a-116">Properties</span></span>
| <span data-ttu-id="9fb8a-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9fb8a-117">Property</span></span>     | <span data-ttu-id="9fb8a-118">Typ</span><span class="sxs-lookup"><span data-stu-id="9fb8a-118">Type</span></span>   |<span data-ttu-id="9fb8a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fb8a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fb8a-120">id</span><span class="sxs-lookup"><span data-stu-id="9fb8a-120">id</span></span>|<span data-ttu-id="9fb8a-121">string</span><span class="sxs-lookup"><span data-stu-id="9fb8a-121">string</span></span>|<span data-ttu-id="9fb8a-p101">Die Eigenschafts-ID, die zum Identifizieren der Eigenschaft verwendet wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9fb8a-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="9fb8a-124">value</span><span class="sxs-lookup"><span data-stu-id="9fb8a-124">value</span></span>|<span data-ttu-id="9fb8a-125">string</span><span class="sxs-lookup"><span data-stu-id="9fb8a-125">string</span></span>|<span data-ttu-id="9fb8a-126">Ein Eigenschaftswert.</span><span class="sxs-lookup"><span data-stu-id="9fb8a-126">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fb8a-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9fb8a-127">Relationships</span></span>
<span data-ttu-id="9fb8a-128">Keine</span><span class="sxs-lookup"><span data-stu-id="9fb8a-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9fb8a-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9fb8a-129">JSON representation</span></span>

<span data-ttu-id="9fb8a-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9fb8a-130">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
