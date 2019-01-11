---
title: singleValueLegacyExtendedProperty-Ressourcentyp
description: 'Eine erweiterte Eigenschaft, die einen einzelnen Wert enthält. '
localization_priority: Normal
ms.openlocfilehash: 51a42661ea3a19ea8e82ba78115bfa5290d99d15
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857414"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="1c15b-103">singleValueLegacyExtendedProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1c15b-103">singleValueLegacyExtendedProperty resource type</span></span>

> <span data-ttu-id="1c15b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1c15b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c15b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c15b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c15b-106">Eine erweiterte Eigenschaft, die einen einzelnen Wert enthält.</span><span class="sxs-lookup"><span data-stu-id="1c15b-106">An extended property that contains a single value.</span></span> 

<span data-ttu-id="1c15b-107">Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="1c15b-107">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="1c15b-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="1c15b-108">Methods</span></span>

| <span data-ttu-id="1c15b-109">Methode</span><span class="sxs-lookup"><span data-stu-id="1c15b-109">Method</span></span>           | <span data-ttu-id="1c15b-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1c15b-110">Return Type</span></span>    |<span data-ttu-id="1c15b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c15b-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1c15b-112">Post</span><span class="sxs-lookup"><span data-stu-id="1c15b-112">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="1c15b-113">Eine Ressourceninstanz der unterstützten: [Nachricht](../resources/message.md), [MailFolder](../resources/mailfolder.md), [Ereignis](../resources/event.md), [Kalender](../resources/calendar.md), [wenden Sie sich an](../resources/contact.md), [ContactFolder](../resources/contactfolder.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md), jedoch nicht der Gruppe [Buchen](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="1c15b-113">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="1c15b-114">Erstellen einer **singleValueLegacyExtendedProperty** in einer neuen oder vorhandenen Instanz einer unterstützten Ressource.</span><span class="sxs-lookup"><span data-stu-id="1c15b-114">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="1c15b-115">Get</span><span class="sxs-lookup"><span data-stu-id="1c15b-115">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="1c15b-116">Eine oder eine Auflistung von unterstützten Ressourceninstanz ([Nachricht](../resources/message.md), [MailFolder](../resources/mailfolder.md), [Ereignis](../resources/event.md), [Kalender](../resources/calendar.md), [wenden Sie sich an](../resources/contact.md), [ContactFolder](../resources/contactfolder.md), [Outlook-Aufgabe](../resources/outlooktask.md), [Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md)oder Gruppe [Buchen](../resources/post.md)), oder eine solche Instanz mit einem [SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) -Objekt erweitert.</span><span class="sxs-lookup"><span data-stu-id="1c15b-116">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="1c15b-117">Abrufen einer Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1c15b-117">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="1c15b-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1c15b-118">Properties</span></span>
| <span data-ttu-id="1c15b-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1c15b-119">Property</span></span>     | <span data-ttu-id="1c15b-120">Typ</span><span class="sxs-lookup"><span data-stu-id="1c15b-120">Type</span></span>   |<span data-ttu-id="1c15b-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c15b-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c15b-122">id</span><span class="sxs-lookup"><span data-stu-id="1c15b-122">id</span></span>|<span data-ttu-id="1c15b-123">string</span><span class="sxs-lookup"><span data-stu-id="1c15b-123">string</span></span>|<span data-ttu-id="1c15b-p102">Die Eigenschaften-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1c15b-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="1c15b-126">value</span><span class="sxs-lookup"><span data-stu-id="1c15b-126">value</span></span>|<span data-ttu-id="1c15b-127">string</span><span class="sxs-lookup"><span data-stu-id="1c15b-127">string</span></span>|<span data-ttu-id="1c15b-128">Ein Eigenschaftswert.</span><span class="sxs-lookup"><span data-stu-id="1c15b-128">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c15b-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1c15b-129">Relationships</span></span>
<span data-ttu-id="1c15b-130">Keine</span><span class="sxs-lookup"><span data-stu-id="1c15b-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1c15b-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1c15b-131">JSON representation</span></span>

<span data-ttu-id="1c15b-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1c15b-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
