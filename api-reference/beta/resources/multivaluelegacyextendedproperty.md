---
title: multiValueLegacyExtendedProperty-Ressourcentyp
description: Eine erweiterte Eigenschaft, die eine Sammlung von Werten enthält.
ms.openlocfilehash: efb871594028b5c2d54b1c081f901717b754c8ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062026"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="ac62d-103">multiValueLegacyExtendedProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ac62d-103">multiValueLegacyExtendedProperty resource type</span></span>

> <span data-ttu-id="ac62d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ac62d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac62d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ac62d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac62d-106">Eine erweiterte Eigenschaft, die eine Sammlung von Werten enthält.</span><span class="sxs-lookup"><span data-stu-id="ac62d-106">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="ac62d-107">Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="ac62d-107">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="ac62d-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="ac62d-108">Methods</span></span>

| <span data-ttu-id="ac62d-109">Methode</span><span class="sxs-lookup"><span data-stu-id="ac62d-109">Method</span></span>           | <span data-ttu-id="ac62d-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ac62d-110">Return Type</span></span>    |<span data-ttu-id="ac62d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac62d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac62d-112">Post</span><span class="sxs-lookup"><span data-stu-id="ac62d-112">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="ac62d-113">Eine Ressourceninstanz der unterstützten: [Nachricht](../resources/message.md), [MailFolder](../resources/mailfolder.md), [Ereignis](../resources/event.md), [Kalender](../resources/calendar.md), [wenden Sie sich an](../resources/contact.md), [ContactFolder](../resources/contactfolder.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ac62d-113">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="ac62d-114">Hinweis: dieser Gruppe [Buchen](../resources/post.md) nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="ac62d-114">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="ac62d-115">Erstellen einer **multiValueLegacyExtendedProperty** in einer neuen oder vorhandenen Instanz einer unterstützten Ressource.</span><span class="sxs-lookup"><span data-stu-id="ac62d-115">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="ac62d-116">Get</span><span class="sxs-lookup"><span data-stu-id="ac62d-116">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="ac62d-117">Eine Ressourceninstanz unterstützte ([Nachricht](../resources/message.md), [MailFolder](../resources/mailfolder.md), [Ereignis](../resources/event.md), [Kalender](../resources/calendar.md), [wenden Sie sich an](../resources/contact.md), [ContactFolder](../resources/contactfolder.md), [Outlook-Aufgabe](../resources/outlooktask.md), [Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md)oder Gruppe [Buchen](../resources/post.md)) erweitert mit einem [ MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) Objekt.</span><span class="sxs-lookup"><span data-stu-id="ac62d-117">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="ac62d-118">Abrufen einer Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="ac62d-118">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac62d-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ac62d-119">Properties</span></span>
| <span data-ttu-id="ac62d-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ac62d-120">Property</span></span>     | <span data-ttu-id="ac62d-121">Typ</span><span class="sxs-lookup"><span data-stu-id="ac62d-121">Type</span></span>   |<span data-ttu-id="ac62d-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac62d-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac62d-123">id</span><span class="sxs-lookup"><span data-stu-id="ac62d-123">id</span></span>|<span data-ttu-id="ac62d-124">string</span><span class="sxs-lookup"><span data-stu-id="ac62d-124">string</span></span>|<span data-ttu-id="ac62d-p103">Die Eigenschaften-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ac62d-p103">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="ac62d-127">value</span><span class="sxs-lookup"><span data-stu-id="ac62d-127">value</span></span>|<span data-ttu-id="ac62d-128">string collection</span><span class="sxs-lookup"><span data-stu-id="ac62d-128">string collection</span></span>|<span data-ttu-id="ac62d-129">Eine Sammlung von Eigenschaftswerten.</span><span class="sxs-lookup"><span data-stu-id="ac62d-129">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac62d-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ac62d-130">Relationships</span></span>
<span data-ttu-id="ac62d-131">Keine</span><span class="sxs-lookup"><span data-stu-id="ac62d-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ac62d-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ac62d-132">JSON representation</span></span>

<span data-ttu-id="ac62d-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ac62d-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.multivaluelegacyextendedproperty"
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