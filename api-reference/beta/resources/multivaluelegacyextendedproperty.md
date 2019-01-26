---
title: multiValueLegacyExtendedProperty-Ressourcentyp
description: Eine erweiterte Eigenschaft, die eine Sammlung von Werten enthält.
localization_priority: Normal
ms.openlocfilehash: de77f94076fe6bb2f0aa3ded3b1839b8d25ce752
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575891"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="e1386-103">multiValueLegacyExtendedProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e1386-103">multiValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1386-104">Eine erweiterte Eigenschaft, die eine Sammlung von Werten enthält.</span><span class="sxs-lookup"><span data-stu-id="e1386-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="e1386-105">Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e1386-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="e1386-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="e1386-106">Methods</span></span>

| <span data-ttu-id="e1386-107">Methode</span><span class="sxs-lookup"><span data-stu-id="e1386-107">Method</span></span>           | <span data-ttu-id="e1386-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e1386-108">Return Type</span></span>    |<span data-ttu-id="e1386-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1386-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e1386-110">Post</span><span class="sxs-lookup"><span data-stu-id="e1386-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="e1386-111">Eine Ressourceninstanz der unterstützten: [Nachricht](../resources/message.md), [MailFolder](../resources/mailfolder.md), [Ereignis](../resources/event.md), [Kalender](../resources/calendar.md), [wenden Sie sich an](../resources/contact.md), [ContactFolder](../resources/contactfolder.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md).</span><span class="sxs-lookup"><span data-stu-id="e1386-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="e1386-112">Hinweis: dieser Gruppe [Buchen](../resources/post.md) nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="e1386-112">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="e1386-113">Erstellen einer **multiValueLegacyExtendedProperty** in einer neuen oder vorhandenen Instanz einer unterstützten Ressource.</span><span class="sxs-lookup"><span data-stu-id="e1386-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="e1386-114">Get</span><span class="sxs-lookup"><span data-stu-id="e1386-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="e1386-115">Eine Ressourceninstanz unterstützte ([Nachricht](../resources/message.md), [MailFolder](../resources/mailfolder.md), [Ereignis](../resources/event.md), [Kalender](../resources/calendar.md), [wenden Sie sich an](../resources/contact.md), [ContactFolder](../resources/contactfolder.md), [Outlook-Aufgabe](../resources/outlooktask.md), [Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md)oder Gruppe [Buchen](../resources/post.md)) erweitert mit einem [ MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) Objekt.</span><span class="sxs-lookup"><span data-stu-id="e1386-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="e1386-116">Abrufen einer Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="e1386-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1386-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e1386-117">Properties</span></span>
| <span data-ttu-id="e1386-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1386-118">Property</span></span>     | <span data-ttu-id="e1386-119">Typ</span><span class="sxs-lookup"><span data-stu-id="e1386-119">Type</span></span>   |<span data-ttu-id="e1386-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1386-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1386-121">id</span><span class="sxs-lookup"><span data-stu-id="e1386-121">id</span></span>|<span data-ttu-id="e1386-122">string</span><span class="sxs-lookup"><span data-stu-id="e1386-122">string</span></span>|<span data-ttu-id="e1386-p102">Die Eigenschaften-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e1386-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="e1386-125">value</span><span class="sxs-lookup"><span data-stu-id="e1386-125">value</span></span>|<span data-ttu-id="e1386-126">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e1386-126">string collection</span></span>|<span data-ttu-id="e1386-127">Eine Sammlung von Eigenschaftswerten.</span><span class="sxs-lookup"><span data-stu-id="e1386-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1386-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e1386-128">Relationships</span></span>
<span data-ttu-id="e1386-129">Keine</span><span class="sxs-lookup"><span data-stu-id="e1386-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e1386-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e1386-130">JSON representation</span></span>

<span data-ttu-id="e1386-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e1386-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/multivaluelegacyextendedproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
