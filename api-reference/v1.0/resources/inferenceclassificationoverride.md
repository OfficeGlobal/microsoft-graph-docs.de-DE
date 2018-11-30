---
title: inferenceClassificationOverride-Ressourcentyp
description: Stellt die Außerkraftsetzung eines Benutzers dafür dar, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen.
ms.openlocfilehash: 3f3f07e870a4ba549062197a380633ab591c54fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017827"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="d528c-103">inferenceClassificationOverride-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d528c-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="d528c-104">Stellt die Außerkraftsetzung eines Benutzers dafür dar, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d528c-104">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="d528c-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d528c-105">Methods</span></span>

| <span data-ttu-id="d528c-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d528c-106">Method</span></span>           | <span data-ttu-id="d528c-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d528c-107">Return Type</span></span>    |<span data-ttu-id="d528c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d528c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d528c-109">Update</span><span class="sxs-lookup"><span data-stu-id="d528c-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="d528c-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="d528c-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="d528c-111">Ändern Sie das **ClassifyAs** -Feld einer Außerkraftsetzung wie angegeben.</span><span class="sxs-lookup"><span data-stu-id="d528c-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="d528c-112">Delete</span><span class="sxs-lookup"><span data-stu-id="d528c-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="d528c-113">Keine</span><span class="sxs-lookup"><span data-stu-id="d528c-113">None</span></span> |<span data-ttu-id="d528c-114">Löscht eine Außerkraftsetzung, die durch ihre ID angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="d528c-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="d528c-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d528c-115">Properties</span></span>
| <span data-ttu-id="d528c-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d528c-116">Property</span></span>     | <span data-ttu-id="d528c-117">Typ</span><span class="sxs-lookup"><span data-stu-id="d528c-117">Type</span></span>   |<span data-ttu-id="d528c-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d528c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d528c-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="d528c-119">classifyAs</span></span>|<span data-ttu-id="d528c-120">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="d528c-120">inferenceClassificationType</span></span>| <span data-ttu-id="d528c-121">Gibt an, wie eingehende-Nachrichten von einer bestimmten Absender sollte stets als klassifiziert werden.</span><span class="sxs-lookup"><span data-stu-id="d528c-121">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="d528c-122">Die möglichen Werte sind: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="d528c-122">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="d528c-123">id</span><span class="sxs-lookup"><span data-stu-id="d528c-123">id</span></span>|<span data-ttu-id="d528c-124">string</span><span class="sxs-lookup"><span data-stu-id="d528c-124">string</span></span>| <span data-ttu-id="d528c-p102">Der eindeutige Bezeichner der Außerkraftsetzung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d528c-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="d528c-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d528c-127">senderEmailAddress</span></span>|[<span data-ttu-id="d528c-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d528c-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="d528c-129">Die E-Mail-Adressinformationen des Absenders, für den die Außerkraftsetzung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="d528c-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d528c-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d528c-130">Relationships</span></span>
<span data-ttu-id="d528c-131">Keine</span><span class="sxs-lookup"><span data-stu-id="d528c-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d528c-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d528c-132">JSON representation</span></span>

<span data-ttu-id="d528c-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d528c-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->