---
title: inferenceClassification-Ressourcentyp
description: 'Klassifizierung der Nachrichten eines Benutzers, um den Fokus auf die Nachrichten zu legen, die für den Benutzer relevanter oder wichtiger sind. '
ms.openlocfilehash: c1536ff2b88b1830c2f2a2bc5a7bed519782df4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058031"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="686b5-103">inferenceClassification-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="686b5-103">inferenceClassification resource type</span></span>

> <span data-ttu-id="686b5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="686b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="686b5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="686b5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="686b5-106">Klassifizierung der Nachrichten eines Benutzers, um den Fokus auf die Nachrichten zu legen, die für den Benutzer relevanter oder wichtiger sind.</span><span class="sxs-lookup"><span data-stu-id="686b5-106">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="686b5-107">Weitere Informationen finden Sie unter [Verwalten eines Posteingang mit Fokus](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="686b5-107">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="686b5-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="686b5-108">Methods</span></span>

| <span data-ttu-id="686b5-109">Methode</span><span class="sxs-lookup"><span data-stu-id="686b5-109">Method</span></span>           | <span data-ttu-id="686b5-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="686b5-110">Return Type</span></span>    |<span data-ttu-id="686b5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="686b5-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="686b5-112">inferenceClassificationOverride erstellen</span><span class="sxs-lookup"><span data-stu-id="686b5-112">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="686b5-113">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="686b5-113">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="686b5-p102">Erstellen einer Außerkraftsetzung für einen Absender, der durch eine SMTP-Adresse identifiziert wird. Künftige Nachrichten von dieser SMTP-Adresse werden durchgängig klassifiziert wie in der Außerkraftsetzung angegeben.</span><span class="sxs-lookup"><span data-stu-id="686b5-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="686b5-116">Außerkraftsetzungen auflisten</span><span class="sxs-lookup"><span data-stu-id="686b5-116">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="686b5-117">[inferenceClassificationOverride-Sammlung](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="686b5-117">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="686b5-118">Dient zum Abrufen der Außerkraftsetzungen, die ein Benutzer eingerichtet hat, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren.</span><span class="sxs-lookup"><span data-stu-id="686b5-118">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="686b5-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="686b5-119">Properties</span></span>
| <span data-ttu-id="686b5-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="686b5-120">Property</span></span>     | <span data-ttu-id="686b5-121">Typ</span><span class="sxs-lookup"><span data-stu-id="686b5-121">Type</span></span>   |<span data-ttu-id="686b5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="686b5-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="686b5-123">id</span><span class="sxs-lookup"><span data-stu-id="686b5-123">id</span></span>|<span data-ttu-id="686b5-124">string</span><span class="sxs-lookup"><span data-stu-id="686b5-124">string</span></span>| <span data-ttu-id="686b5-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="686b5-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="686b5-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="686b5-126">Relationships</span></span>
| <span data-ttu-id="686b5-127">Beziehung</span><span class="sxs-lookup"><span data-stu-id="686b5-127">Relationship</span></span> | <span data-ttu-id="686b5-128">Typ</span><span class="sxs-lookup"><span data-stu-id="686b5-128">Type</span></span>   |<span data-ttu-id="686b5-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="686b5-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="686b5-130">Außerkraftsetzungen</span><span class="sxs-lookup"><span data-stu-id="686b5-130">overrides</span></span>|<span data-ttu-id="686b5-131">[inferenceClassificationOverride-Sammlung](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="686b5-131">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="686b5-p103">Eine Reihe von Außerkraftsetzungen für einen Benutzer, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren: `focused` oder `other`. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="686b5-p103">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="686b5-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="686b5-135">JSON representation</span></span>

<span data-ttu-id="686b5-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="686b5-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassification"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->