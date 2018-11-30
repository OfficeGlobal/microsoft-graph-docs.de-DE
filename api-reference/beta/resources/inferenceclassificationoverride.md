---
title: inferenceClassificationOverride-Ressourcentyp
description: Stellt sollte Außerkraftsetzung für eingehende von einem bestimmten Absender wie Nachrichten des Benutzers immer als klassifiziert werden
ms.openlocfilehash: 63c753b7af21907717d7d9706d0606726d5670f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059189"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="f27d5-103">inferenceClassificationOverride-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f27d5-103">inferenceClassificationOverride resource type</span></span>

> <span data-ttu-id="f27d5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f27d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f27d5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f27d5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f27d5-106">Stellt einen Benutzer außer Kraft setzen für eingehende wie von einem bestimmten Absender Nachrichten wie in eine [Praxisorientierte Posteingang](manage-focused-inbox.md)immer klassifiziert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f27d5-106">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="f27d5-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="f27d5-107">Methods</span></span>

| <span data-ttu-id="f27d5-108">Methode</span><span class="sxs-lookup"><span data-stu-id="f27d5-108">Method</span></span>           | <span data-ttu-id="f27d5-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f27d5-109">Return Type</span></span>    |<span data-ttu-id="f27d5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f27d5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f27d5-111">Update</span><span class="sxs-lookup"><span data-stu-id="f27d5-111">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="f27d5-112">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="f27d5-112">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="f27d5-113">Ändern Sie das **ClassifyAs** -Feld einer Außerkraftsetzung wie angegeben.</span><span class="sxs-lookup"><span data-stu-id="f27d5-113">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="f27d5-114">Delete</span><span class="sxs-lookup"><span data-stu-id="f27d5-114">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="f27d5-115">Keine</span><span class="sxs-lookup"><span data-stu-id="f27d5-115">None</span></span> |<span data-ttu-id="f27d5-116">Löscht eine Außerkraftsetzung, die durch ihre ID angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="f27d5-116">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="f27d5-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f27d5-117">Properties</span></span>
| <span data-ttu-id="f27d5-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f27d5-118">Property</span></span>     | <span data-ttu-id="f27d5-119">Typ</span><span class="sxs-lookup"><span data-stu-id="f27d5-119">Type</span></span>   |<span data-ttu-id="f27d5-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f27d5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f27d5-121">classifyAs</span><span class="sxs-lookup"><span data-stu-id="f27d5-121">classifyAs</span></span>|<span data-ttu-id="f27d5-122">string</span><span class="sxs-lookup"><span data-stu-id="f27d5-122">string</span></span>| <span data-ttu-id="f27d5-p102">Gibt an, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen. Mögliche Werte: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="f27d5-p102">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="f27d5-125">id</span><span class="sxs-lookup"><span data-stu-id="f27d5-125">id</span></span>|<span data-ttu-id="f27d5-126">string</span><span class="sxs-lookup"><span data-stu-id="f27d5-126">string</span></span>| <span data-ttu-id="f27d5-p103">Der eindeutige Bezeichner der Außerkraftsetzung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f27d5-p103">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="f27d5-129">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f27d5-129">senderEmailAddress</span></span>|[<span data-ttu-id="f27d5-130">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f27d5-130">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="f27d5-131">Die E-Mail-Adressinformationen des Absenders, für den die Außerkraftsetzung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="f27d5-131">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f27d5-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f27d5-132">Relationships</span></span>
<span data-ttu-id="f27d5-133">Keine</span><span class="sxs-lookup"><span data-stu-id="f27d5-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f27d5-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f27d5-134">JSON representation</span></span>

<span data-ttu-id="f27d5-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f27d5-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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