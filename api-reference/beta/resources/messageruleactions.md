---
title: messageRuleActions-Ressourcentyp
description: Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a786a225bb9d439d60a29d2395b2d438975fc16c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523232"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="b00e3-103">messageRuleActions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b00e3-103">messageRuleActions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b00e3-104">Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="b00e3-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="b00e3-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b00e3-105">Properties</span></span>
| <span data-ttu-id="b00e3-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b00e3-106">Property</span></span>     | <span data-ttu-id="b00e3-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b00e3-107">Type</span></span>   |<span data-ttu-id="b00e3-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b00e3-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b00e3-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="b00e3-109">assignCategories</span></span> | <span data-ttu-id="b00e3-110">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b00e3-110">String collection</span></span> | <span data-ttu-id="b00e3-111">Eine Liste von Kategorien, die einer Nachricht zugewiesen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b00e3-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="b00e3-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="b00e3-112">copyToFolder</span></span> | <span data-ttu-id="b00e3-113">String</span><span class="sxs-lookup"><span data-stu-id="b00e3-113">String</span></span> | <span data-ttu-id="b00e3-114">Die ID eines Ordners, in den eine Nachricht kopiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b00e3-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="b00e3-115">Löschen</span><span class="sxs-lookup"><span data-stu-id="b00e3-115">delete</span></span> | <span data-ttu-id="b00e3-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b00e3-116">Boolean</span></span> | <span data-ttu-id="b00e3-117">Gibt an, ob eine Nachricht in den Ordner „Gelöschte Elemente“ verschoben werden soll.</span><span class="sxs-lookup"><span data-stu-id="b00e3-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="b00e3-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="b00e3-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="b00e3-119">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="b00e3-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="b00e3-120">Die E-Mail-Adressen der Empfänger, an die eine Nachricht als Anlage weitergeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b00e3-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="b00e3-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="b00e3-121">forwardTo</span></span> | <span data-ttu-id="b00e3-122">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b00e3-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="b00e3-123">Die E-Mail-Adressen der Empfänger, an die eine Nachricht weitergeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b00e3-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="b00e3-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="b00e3-124">markAsRead</span></span> | <span data-ttu-id="b00e3-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b00e3-125">Boolean</span></span> | <span data-ttu-id="b00e3-126">Gibt an, ob eine Nachricht als gelesen markiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b00e3-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="b00e3-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="b00e3-127">markImportance</span></span> | <span data-ttu-id="b00e3-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b00e3-128">String</span></span> | <span data-ttu-id="b00e3-129">Legt die Wichtigkeit der Nachricht fest. Die folgenden Einstellungen sind möglich: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b00e3-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="b00e3-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="b00e3-130">moveToFolder</span></span> |  <span data-ttu-id="b00e3-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b00e3-131">String</span></span>| <span data-ttu-id="b00e3-132">Die ID des Ordners, in den eine Nachricht verschoben wird.</span><span class="sxs-lookup"><span data-stu-id="b00e3-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="b00e3-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="b00e3-133">permanentDelete</span></span> | <span data-ttu-id="b00e3-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b00e3-134">Boolean</span></span> | <span data-ttu-id="b00e3-135">Gibt an, ob eine Nachricht dauerhaft gelöscht und nicht im Ordner „Gelöschte Elemente“ gespeichert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b00e3-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="b00e3-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="b00e3-136">redirectTo</span></span> | [<span data-ttu-id="b00e3-137">recipient</span><span class="sxs-lookup"><span data-stu-id="b00e3-137">recipient</span></span>](recipient.md) | <span data-ttu-id="b00e3-138">Die E-Mail-Adresse, an die eine Nachricht umgeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b00e3-138">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="b00e3-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="b00e3-139">stopProcessingRules</span></span> | <span data-ttu-id="b00e3-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b00e3-140">Boolean</span></span> | <span data-ttu-id="b00e3-141">Gibt an, ob nachfolgende Regeln ausgewertet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b00e3-141">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b00e3-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b00e3-142">JSON representation</span></span>
<span data-ttu-id="b00e3-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b00e3-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": {"@odata.type": "microsoft.graph.recipient"},
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messageruleactions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
