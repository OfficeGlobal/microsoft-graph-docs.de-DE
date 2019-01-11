---
title: inferenceClassification-Ressourcentyp
description: 'Klassifizierung der Nachrichten eines Benutzers, um den Fokus auf die Nachrichten zu legen, die für den Benutzer relevanter oder wichtiger sind. '
localization_priority: Normal
ms.openlocfilehash: 8dfd76b31e452532181b46cdb0b5c321e92273a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840726"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="fdb10-103">inferenceClassification-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fdb10-103">inferenceClassification resource type</span></span>

<span data-ttu-id="fdb10-104">Klassifizierung der Nachrichten eines Benutzers, um den Fokus auf die Nachrichten zu legen, die für den Benutzer relevanter oder wichtiger sind.</span><span class="sxs-lookup"><span data-stu-id="fdb10-104">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="fdb10-105">Weitere Informationen finden Sie unter [Verwalten eines Posteingang mit Fokus](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="fdb10-105">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="fdb10-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="fdb10-106">Methods</span></span>

| <span data-ttu-id="fdb10-107">Methode</span><span class="sxs-lookup"><span data-stu-id="fdb10-107">Method</span></span>           | <span data-ttu-id="fdb10-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fdb10-108">Return Type</span></span>    |<span data-ttu-id="fdb10-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdb10-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fdb10-110">inferenceClassificationOverride erstellen</span><span class="sxs-lookup"><span data-stu-id="fdb10-110">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="fdb10-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="fdb10-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="fdb10-p101">Erstellen einer Außerkraftsetzung für einen Absender, der durch eine SMTP-Adresse identifiziert wird. Künftige Nachrichten von dieser SMTP-Adresse werden durchgängig klassifiziert wie in der Außerkraftsetzung angegeben.</span><span class="sxs-lookup"><span data-stu-id="fdb10-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="fdb10-114">Außerkraftsetzungen auflisten</span><span class="sxs-lookup"><span data-stu-id="fdb10-114">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="fdb10-115">[inferenceClassificationOverride-Sammlung](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="fdb10-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="fdb10-116">Dient zum Abrufen der Außerkraftsetzungen, die ein Benutzer eingerichtet hat, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren.</span><span class="sxs-lookup"><span data-stu-id="fdb10-116">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="fdb10-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fdb10-117">Properties</span></span>
| <span data-ttu-id="fdb10-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fdb10-118">Property</span></span>     | <span data-ttu-id="fdb10-119">Typ</span><span class="sxs-lookup"><span data-stu-id="fdb10-119">Type</span></span>   |<span data-ttu-id="fdb10-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdb10-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdb10-121">id</span><span class="sxs-lookup"><span data-stu-id="fdb10-121">id</span></span>|<span data-ttu-id="fdb10-122">string</span><span class="sxs-lookup"><span data-stu-id="fdb10-122">string</span></span>| <span data-ttu-id="fdb10-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fdb10-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdb10-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fdb10-124">Relationships</span></span>
| <span data-ttu-id="fdb10-125">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fdb10-125">Relationship</span></span> | <span data-ttu-id="fdb10-126">Typ</span><span class="sxs-lookup"><span data-stu-id="fdb10-126">Type</span></span>   |<span data-ttu-id="fdb10-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdb10-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdb10-128">Außerkraftsetzungen</span><span class="sxs-lookup"><span data-stu-id="fdb10-128">overrides</span></span>|<span data-ttu-id="fdb10-129">[inferenceClassificationOverride-Sammlung](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="fdb10-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="fdb10-p102">Eine Reihe von Außerkraftsetzungen für einen Benutzer, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren: `focused` oder `other`. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="fdb10-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdb10-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fdb10-133">JSON representation</span></span>

<span data-ttu-id="fdb10-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fdb10-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
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
