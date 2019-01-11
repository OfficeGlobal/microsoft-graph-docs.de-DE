---
title: multiValueLegacyExtendedProperty-Ressourcentyp
description: Eine erweiterte Eigenschaft, die eine Sammlung von Werten enthält.
localization_priority: Normal
ms.openlocfilehash: 87823559bad3e149ef3c4d4d6f21f43cf66c41fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827034"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="dfa84-103">multiValueLegacyExtendedProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dfa84-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="dfa84-104">Eine erweiterte Eigenschaft, die eine Sammlung von Werten enthält.</span><span class="sxs-lookup"><span data-stu-id="dfa84-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="dfa84-105">Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="dfa84-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="dfa84-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="dfa84-106">Methods</span></span>

| <span data-ttu-id="dfa84-107">Methode</span><span class="sxs-lookup"><span data-stu-id="dfa84-107">Method</span></span>           | <span data-ttu-id="dfa84-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="dfa84-108">Return Type</span></span>    |<span data-ttu-id="dfa84-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dfa84-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dfa84-110">Post</span><span class="sxs-lookup"><span data-stu-id="dfa84-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="dfa84-p101">Eine unterstützte Ressourceninstanz: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) oder [contactFolder](../resources/contactfolder.md). Beachten Sie, dass [post](../resources/post.md) für die Gruppe nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="dfa84-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="dfa84-113">Erstellen einer **multiValueLegacyExtendedProperty** in einer neuen oder vorhandenen Instanz einer unterstützten Ressource.</span><span class="sxs-lookup"><span data-stu-id="dfa84-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="dfa84-114">Get</span><span class="sxs-lookup"><span data-stu-id="dfa84-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="dfa84-115">Eine unterstützte Ressourceninstanz ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) oder [post](../resources/post.md) für die Gruppe), erweitert mit einem [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="dfa84-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="dfa84-116">Abrufen einer Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="dfa84-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="dfa84-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dfa84-117">Properties</span></span>
| <span data-ttu-id="dfa84-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dfa84-118">Property</span></span>     | <span data-ttu-id="dfa84-119">Typ</span><span class="sxs-lookup"><span data-stu-id="dfa84-119">Type</span></span>   |<span data-ttu-id="dfa84-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dfa84-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfa84-121">id</span><span class="sxs-lookup"><span data-stu-id="dfa84-121">id</span></span>|<span data-ttu-id="dfa84-122">string</span><span class="sxs-lookup"><span data-stu-id="dfa84-122">string</span></span>|<span data-ttu-id="dfa84-p102">Die Eigenschaften-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dfa84-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="dfa84-125">value</span><span class="sxs-lookup"><span data-stu-id="dfa84-125">value</span></span>|<span data-ttu-id="dfa84-126">string collection</span><span class="sxs-lookup"><span data-stu-id="dfa84-126">string collection</span></span>|<span data-ttu-id="dfa84-127">Eine Sammlung von Eigenschaftswerten.</span><span class="sxs-lookup"><span data-stu-id="dfa84-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfa84-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dfa84-128">Relationships</span></span>
<span data-ttu-id="dfa84-129">Keine</span><span class="sxs-lookup"><span data-stu-id="dfa84-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dfa84-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dfa84-130">JSON representation</span></span>

<span data-ttu-id="dfa84-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dfa84-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
