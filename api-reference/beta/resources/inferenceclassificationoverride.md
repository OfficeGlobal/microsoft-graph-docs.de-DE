---
title: inferenceClassificationOverride-Ressourcentyp
description: Stellt die Außerkraftsetzung eines Benutzers dafür dar, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen.
localization_priority: Normal
ms.openlocfilehash: 1cf1896b43dccfe59ed253c22a8a7341e9ee6e1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511800"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="bbe1b-103">inferenceClassificationOverride-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bbe1b-103">inferenceClassificationOverride resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbe1b-104">Stellt einen Benutzer außer Kraft setzen für eingehende wie von einem bestimmten Absender Nachrichten wie in eine [Praxisorientierte Posteingang](manage-focused-inbox.md)immer klassifiziert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-104">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="bbe1b-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="bbe1b-105">Methods</span></span>

| <span data-ttu-id="bbe1b-106">Methode</span><span class="sxs-lookup"><span data-stu-id="bbe1b-106">Method</span></span>           | <span data-ttu-id="bbe1b-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bbe1b-107">Return Type</span></span>    |<span data-ttu-id="bbe1b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbe1b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bbe1b-109">Update</span><span class="sxs-lookup"><span data-stu-id="bbe1b-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="bbe1b-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="bbe1b-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="bbe1b-111">Ändert das **classifyAs**-Feld einer Außerkraftsetzung wie angegeben.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="bbe1b-112">Delete</span><span class="sxs-lookup"><span data-stu-id="bbe1b-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="bbe1b-113">Keine</span><span class="sxs-lookup"><span data-stu-id="bbe1b-113">None</span></span> |<span data-ttu-id="bbe1b-114">Löscht eine Außerkraftsetzung, die durch ihre ID angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="bbe1b-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bbe1b-115">Properties</span></span>
| <span data-ttu-id="bbe1b-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bbe1b-116">Property</span></span>     | <span data-ttu-id="bbe1b-117">Typ</span><span class="sxs-lookup"><span data-stu-id="bbe1b-117">Type</span></span>   |<span data-ttu-id="bbe1b-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbe1b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbe1b-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="bbe1b-119">classifyAs</span></span>|<span data-ttu-id="bbe1b-120">string</span><span class="sxs-lookup"><span data-stu-id="bbe1b-120">string</span></span>| <span data-ttu-id="bbe1b-p101">Gibt an, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen. Mögliche Werte: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="bbe1b-123">id</span><span class="sxs-lookup"><span data-stu-id="bbe1b-123">id</span></span>|<span data-ttu-id="bbe1b-124">string</span><span class="sxs-lookup"><span data-stu-id="bbe1b-124">string</span></span>| <span data-ttu-id="bbe1b-p102">Der eindeutige Bezeichner der Außerkraftsetzung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="bbe1b-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="bbe1b-127">senderEmailAddress</span></span>|[<span data-ttu-id="bbe1b-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bbe1b-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="bbe1b-129">Die E-Mail-Adressinformationen des Absenders, für den die Außerkraftsetzung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbe1b-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bbe1b-130">Relationships</span></span>
<span data-ttu-id="bbe1b-131">Keine</span><span class="sxs-lookup"><span data-stu-id="bbe1b-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bbe1b-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bbe1b-132">JSON representation</span></span>

<span data-ttu-id="bbe1b-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-133">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/inferenceclassificationoverride.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
