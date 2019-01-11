---
title: messageRuleActions-Ressourcentyp
description: Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: f92c253b400a5164c1def570daef6307c0f4a8bf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876545"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="dc5ac-103">messageRuleActions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dc5ac-103">messageRuleActions resource type</span></span>


<span data-ttu-id="dc5ac-104">Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="dc5ac-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dc5ac-105">Properties</span></span>
| <span data-ttu-id="dc5ac-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dc5ac-106">Property</span></span>     | <span data-ttu-id="dc5ac-107">Typ</span><span class="sxs-lookup"><span data-stu-id="dc5ac-107">Type</span></span>   |<span data-ttu-id="dc5ac-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dc5ac-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dc5ac-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="dc5ac-109">assignCategories</span></span> | <span data-ttu-id="dc5ac-110">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="dc5ac-110">String collection</span></span> | <span data-ttu-id="dc5ac-111">Eine Liste von Kategorien, die einer Nachricht zugewiesen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="dc5ac-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="dc5ac-112">copyToFolder</span></span> | <span data-ttu-id="dc5ac-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc5ac-113">String</span></span> | <span data-ttu-id="dc5ac-114">Die ID eines Ordners, in den eine Nachricht kopiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="dc5ac-115">Löschen</span><span class="sxs-lookup"><span data-stu-id="dc5ac-115">delete</span></span> | <span data-ttu-id="dc5ac-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc5ac-116">Boolean</span></span> | <span data-ttu-id="dc5ac-117">Gibt an, ob eine Nachricht in den Ordner „Gelöschte Elemente“ verschoben werden soll.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="dc5ac-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="dc5ac-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="dc5ac-119">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="dc5ac-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="dc5ac-120">Die E-Mail-Adressen der Empfänger, an die eine Nachricht als Anlage weitergeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="dc5ac-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="dc5ac-121">forwardTo</span></span> | <span data-ttu-id="dc5ac-122">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="dc5ac-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="dc5ac-123">Die E-Mail-Adressen der Empfänger, an die eine Nachricht weitergeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="dc5ac-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="dc5ac-124">markAsRead</span></span> | <span data-ttu-id="dc5ac-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc5ac-125">Boolean</span></span> | <span data-ttu-id="dc5ac-126">Gibt an, ob eine Nachricht als gelesen markiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="dc5ac-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="dc5ac-127">markImportance</span></span> | <span data-ttu-id="dc5ac-128">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="dc5ac-128">importance</span></span> | <span data-ttu-id="dc5ac-129">Legt die Wichtigkeit der Nachricht fest. Die folgenden Einstellungen sind möglich: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="dc5ac-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="dc5ac-130">moveToFolder</span></span> |  <span data-ttu-id="dc5ac-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc5ac-131">String</span></span>| <span data-ttu-id="dc5ac-132">Die ID des Ordners, in den eine Nachricht verschoben wird.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="dc5ac-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="dc5ac-133">permanentDelete</span></span> | <span data-ttu-id="dc5ac-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc5ac-134">Boolean</span></span> | <span data-ttu-id="dc5ac-135">Gibt an, ob eine Nachricht dauerhaft gelöscht und nicht im Ordner „Gelöschte Elemente“ gespeichert werden soll.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="dc5ac-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="dc5ac-136">redirectTo</span></span> | <span data-ttu-id="dc5ac-137">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="dc5ac-137">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="dc5ac-138">Die e-Mail-Adressen in denen eine Nachricht umgeleitet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-138">The email addresses to which a message should be redirected.</span></span> |
| <span data-ttu-id="dc5ac-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="dc5ac-139">stopProcessingRules</span></span> | <span data-ttu-id="dc5ac-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc5ac-140">Boolean</span></span> | <span data-ttu-id="dc5ac-141">Gibt an, ob nachfolgende Regeln ausgewertet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-141">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dc5ac-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dc5ac-142">JSON representation</span></span>
<span data-ttu-id="dc5ac-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dc5ac-143">Here is a JSON representation of the resource.</span></span>

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
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
