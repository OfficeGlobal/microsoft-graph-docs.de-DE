---
title: inferenceClassification-Ressourcentyp
description: 'Klassifizierung der Nachrichten eines Benutzers, um den Fokus auf die Nachrichten zu legen, die für den Benutzer relevanter oder wichtiger sind. '
localization_priority: Normal
ms.openlocfilehash: 82d16e24e21231b8ec168eda793257ef780c2219
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877791"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="77faf-103">inferenceClassification-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="77faf-103">inferenceClassification resource type</span></span>

> <span data-ttu-id="77faf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="77faf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77faf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77faf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77faf-106">Klassifizierung der Nachrichten eines Benutzers, um den Fokus auf die Nachrichten zu legen, die für den Benutzer relevanter oder wichtiger sind.</span><span class="sxs-lookup"><span data-stu-id="77faf-106">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="77faf-107">Weitere Informationen finden Sie unter [Verwalten eines Posteingang mit Fokus](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="77faf-107">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="77faf-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="77faf-108">Methods</span></span>

| <span data-ttu-id="77faf-109">Methode</span><span class="sxs-lookup"><span data-stu-id="77faf-109">Method</span></span>           | <span data-ttu-id="77faf-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="77faf-110">Return Type</span></span>    |<span data-ttu-id="77faf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77faf-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77faf-112">inferenceClassificationOverride erstellen</span><span class="sxs-lookup"><span data-stu-id="77faf-112">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="77faf-113">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="77faf-113">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="77faf-p102">Erstellen einer Außerkraftsetzung für einen Absender, der durch eine SMTP-Adresse identifiziert wird. Künftige Nachrichten von dieser SMTP-Adresse werden durchgängig klassifiziert wie in der Außerkraftsetzung angegeben.</span><span class="sxs-lookup"><span data-stu-id="77faf-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="77faf-116">Außerkraftsetzungen auflisten</span><span class="sxs-lookup"><span data-stu-id="77faf-116">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="77faf-117">[inferenceClassificationOverride-Sammlung](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="77faf-117">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="77faf-118">Dient zum Abrufen der Außerkraftsetzungen, die ein Benutzer eingerichtet hat, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren.</span><span class="sxs-lookup"><span data-stu-id="77faf-118">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="77faf-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77faf-119">Properties</span></span>
| <span data-ttu-id="77faf-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77faf-120">Property</span></span>     | <span data-ttu-id="77faf-121">Typ</span><span class="sxs-lookup"><span data-stu-id="77faf-121">Type</span></span>   |<span data-ttu-id="77faf-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77faf-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77faf-123">id</span><span class="sxs-lookup"><span data-stu-id="77faf-123">id</span></span>|<span data-ttu-id="77faf-124">string</span><span class="sxs-lookup"><span data-stu-id="77faf-124">string</span></span>| <span data-ttu-id="77faf-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="77faf-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77faf-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="77faf-126">Relationships</span></span>
| <span data-ttu-id="77faf-127">Beziehung</span><span class="sxs-lookup"><span data-stu-id="77faf-127">Relationship</span></span> | <span data-ttu-id="77faf-128">Typ</span><span class="sxs-lookup"><span data-stu-id="77faf-128">Type</span></span>   |<span data-ttu-id="77faf-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77faf-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77faf-130">Außerkraftsetzungen</span><span class="sxs-lookup"><span data-stu-id="77faf-130">overrides</span></span>|<span data-ttu-id="77faf-131">[inferenceClassificationOverride-Sammlung](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="77faf-131">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="77faf-p103">Eine Reihe von Außerkraftsetzungen für einen Benutzer, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren: `focused` oder `other`. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="77faf-p103">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77faf-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77faf-135">JSON representation</span></span>

<span data-ttu-id="77faf-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77faf-136">Here is a JSON representation of the resource.</span></span>

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
