---
title: messageRuleActions-Ressourcentyp
description: Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: f6a78442dc82cade6b7e6d9a793fb6e49b3a1beb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889040"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="e843a-103">messageRuleActions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e843a-103">messageRuleActions resource type</span></span>

> <span data-ttu-id="e843a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e843a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e843a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e843a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e843a-106">Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="e843a-106">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="e843a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e843a-107">Properties</span></span>
| <span data-ttu-id="e843a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e843a-108">Property</span></span>     | <span data-ttu-id="e843a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e843a-109">Type</span></span>   |<span data-ttu-id="e843a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e843a-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e843a-111">assignCategories</span><span class="sxs-lookup"><span data-stu-id="e843a-111">assignCategories</span></span> | <span data-ttu-id="e843a-112">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e843a-112">String collection</span></span> | <span data-ttu-id="e843a-113">Eine Liste von Kategorien, die einer Nachricht zugewiesen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e843a-113">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="e843a-114">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="e843a-114">copyToFolder</span></span> | <span data-ttu-id="e843a-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e843a-115">String</span></span> | <span data-ttu-id="e843a-116">Die ID eines Ordners, in den eine Nachricht kopiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e843a-116">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="e843a-117">Löschen</span><span class="sxs-lookup"><span data-stu-id="e843a-117">delete</span></span> | <span data-ttu-id="e843a-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e843a-118">Boolean</span></span> | <span data-ttu-id="e843a-119">Gibt an, ob eine Nachricht in den Ordner „Gelöschte Elemente“ verschoben werden soll.</span><span class="sxs-lookup"><span data-stu-id="e843a-119">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="e843a-120">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="e843a-120">forwardAsAttachmentTo</span></span> | <span data-ttu-id="e843a-121">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e843a-121">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="e843a-122">Die E-Mail-Adressen der Empfänger, an die eine Nachricht als Anlage weitergeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e843a-122">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="e843a-123">forwardTo</span><span class="sxs-lookup"><span data-stu-id="e843a-123">forwardTo</span></span> | <span data-ttu-id="e843a-124">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e843a-124">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="e843a-125">Die E-Mail-Adressen der Empfänger, an die eine Nachricht weitergeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e843a-125">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="e843a-126">markAsRead</span><span class="sxs-lookup"><span data-stu-id="e843a-126">markAsRead</span></span> | <span data-ttu-id="e843a-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e843a-127">Boolean</span></span> | <span data-ttu-id="e843a-128">Gibt an, ob eine Nachricht als gelesen markiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e843a-128">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="e843a-129">markImportance</span><span class="sxs-lookup"><span data-stu-id="e843a-129">markImportance</span></span> | <span data-ttu-id="e843a-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e843a-130">String</span></span> | <span data-ttu-id="e843a-131">Legt die Wichtigkeit der Nachricht fest. Die folgenden Einstellungen sind möglich: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="e843a-131">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="e843a-132">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="e843a-132">moveToFolder</span></span> |  <span data-ttu-id="e843a-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e843a-133">String</span></span>| <span data-ttu-id="e843a-134">Die ID des Ordners, in den eine Nachricht verschoben wird.</span><span class="sxs-lookup"><span data-stu-id="e843a-134">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="e843a-135">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="e843a-135">permanentDelete</span></span> | <span data-ttu-id="e843a-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e843a-136">Boolean</span></span> | <span data-ttu-id="e843a-137">Gibt an, ob eine Nachricht dauerhaft gelöscht und nicht im Ordner „Gelöschte Elemente“ gespeichert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e843a-137">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="e843a-138">redirectTo</span><span class="sxs-lookup"><span data-stu-id="e843a-138">redirectTo</span></span> | [<span data-ttu-id="e843a-139">recipient</span><span class="sxs-lookup"><span data-stu-id="e843a-139">recipient</span></span>](recipient.md) | <span data-ttu-id="e843a-140">Die E-Mail-Adresse, an die eine Nachricht umgeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e843a-140">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="e843a-141">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="e843a-141">stopProcessingRules</span></span> | <span data-ttu-id="e843a-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e843a-142">Boolean</span></span> | <span data-ttu-id="e843a-143">Gibt an, ob nachfolgende Regeln ausgewertet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e843a-143">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e843a-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e843a-144">JSON representation</span></span>
<span data-ttu-id="e843a-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e843a-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
