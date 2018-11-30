---
title: multiValueLegacyExtendedProperty-Ressourcentyp
description: Eine erweiterte Eigenschaft, die eine Sammlung von Werten enthält.
ms.openlocfilehash: 9aa94465ca1a0fb30c4461b99336040c72e2c5c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017273"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="3a8c7-103">multiValueLegacyExtendedProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3a8c7-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="3a8c7-104">Eine erweiterte Eigenschaft, die eine Sammlung von Werten enthält.</span><span class="sxs-lookup"><span data-stu-id="3a8c7-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="3a8c7-105">Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="3a8c7-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="3a8c7-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="3a8c7-106">Methods</span></span>

| <span data-ttu-id="3a8c7-107">Methode</span><span class="sxs-lookup"><span data-stu-id="3a8c7-107">Method</span></span>           | <span data-ttu-id="3a8c7-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3a8c7-108">Return Type</span></span>    |<span data-ttu-id="3a8c7-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a8c7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3a8c7-110">Post</span><span class="sxs-lookup"><span data-stu-id="3a8c7-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="3a8c7-p101">Eine unterstützte Ressourceninstanz: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) oder [contactFolder](../resources/contactfolder.md). Beachten Sie, dass [post](../resources/post.md) für die Gruppe nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="3a8c7-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="3a8c7-113">Erstellen einer **multiValueLegacyExtendedProperty** in einer neuen oder vorhandenen Instanz einer unterstützten Ressource.</span><span class="sxs-lookup"><span data-stu-id="3a8c7-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="3a8c7-114">Get</span><span class="sxs-lookup"><span data-stu-id="3a8c7-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="3a8c7-115">Eine unterstützte Ressourceninstanz ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) oder [post](../resources/post.md) für die Gruppe), erweitert mit einem [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="3a8c7-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="3a8c7-116">Abrufen einer Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="3a8c7-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="3a8c7-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3a8c7-117">Properties</span></span>
| <span data-ttu-id="3a8c7-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3a8c7-118">Property</span></span>     | <span data-ttu-id="3a8c7-119">Typ</span><span class="sxs-lookup"><span data-stu-id="3a8c7-119">Type</span></span>   |<span data-ttu-id="3a8c7-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a8c7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a8c7-121">id</span><span class="sxs-lookup"><span data-stu-id="3a8c7-121">id</span></span>|<span data-ttu-id="3a8c7-122">string</span><span class="sxs-lookup"><span data-stu-id="3a8c7-122">string</span></span>|<span data-ttu-id="3a8c7-p102">Die Eigenschaften-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3a8c7-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="3a8c7-125">value</span><span class="sxs-lookup"><span data-stu-id="3a8c7-125">value</span></span>|<span data-ttu-id="3a8c7-126">string collection</span><span class="sxs-lookup"><span data-stu-id="3a8c7-126">string collection</span></span>|<span data-ttu-id="3a8c7-127">Eine Sammlung von Eigenschaftswerten.</span><span class="sxs-lookup"><span data-stu-id="3a8c7-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a8c7-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3a8c7-128">Relationships</span></span>
<span data-ttu-id="3a8c7-129">Keine</span><span class="sxs-lookup"><span data-stu-id="3a8c7-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3a8c7-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3a8c7-130">JSON representation</span></span>

<span data-ttu-id="3a8c7-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3a8c7-131">Here is a JSON representation of the resource.</span></span>

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