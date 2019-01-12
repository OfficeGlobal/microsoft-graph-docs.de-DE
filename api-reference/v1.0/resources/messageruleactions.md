---
title: messageRuleActions-Ressourcentyp
description: Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 33f1167d7317f941ebfa79b372e9cf575c14989b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914157"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="86403-103">messageRuleActions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="86403-103">messageRuleActions resource type</span></span>


<span data-ttu-id="86403-104">Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="86403-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="86403-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="86403-105">Properties</span></span>
| <span data-ttu-id="86403-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86403-106">Property</span></span>     | <span data-ttu-id="86403-107">Typ</span><span class="sxs-lookup"><span data-stu-id="86403-107">Type</span></span>   |<span data-ttu-id="86403-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86403-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="86403-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="86403-109">assignCategories</span></span> | <span data-ttu-id="86403-110">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="86403-110">String collection</span></span> | <span data-ttu-id="86403-111">Eine Liste von Kategorien, die einer Nachricht zugewiesen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="86403-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="86403-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="86403-112">copyToFolder</span></span> | <span data-ttu-id="86403-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86403-113">String</span></span> | <span data-ttu-id="86403-114">Die ID eines Ordners, in den eine Nachricht kopiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="86403-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="86403-115">Löschen</span><span class="sxs-lookup"><span data-stu-id="86403-115">delete</span></span> | <span data-ttu-id="86403-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86403-116">Boolean</span></span> | <span data-ttu-id="86403-117">Gibt an, ob eine Nachricht in den Ordner „Gelöschte Elemente“ verschoben werden soll.</span><span class="sxs-lookup"><span data-stu-id="86403-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="86403-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="86403-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="86403-119">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="86403-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="86403-120">Die E-Mail-Adressen der Empfänger, an die eine Nachricht als Anlage weitergeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="86403-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="86403-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="86403-121">forwardTo</span></span> | <span data-ttu-id="86403-122">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="86403-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="86403-123">Die E-Mail-Adressen der Empfänger, an die eine Nachricht weitergeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="86403-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="86403-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="86403-124">markAsRead</span></span> | <span data-ttu-id="86403-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86403-125">Boolean</span></span> | <span data-ttu-id="86403-126">Gibt an, ob eine Nachricht als gelesen markiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="86403-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="86403-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="86403-127">markImportance</span></span> | <span data-ttu-id="86403-128">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="86403-128">importance</span></span> | <span data-ttu-id="86403-129">Legt die Wichtigkeit der Nachricht fest. Die folgenden Einstellungen sind möglich: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="86403-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="86403-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="86403-130">moveToFolder</span></span> |  <span data-ttu-id="86403-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86403-131">String</span></span>| <span data-ttu-id="86403-132">Die ID des Ordners, in den eine Nachricht verschoben wird.</span><span class="sxs-lookup"><span data-stu-id="86403-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="86403-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="86403-133">permanentDelete</span></span> | <span data-ttu-id="86403-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86403-134">Boolean</span></span> | <span data-ttu-id="86403-135">Gibt an, ob eine Nachricht dauerhaft gelöscht und nicht im Ordner „Gelöschte Elemente“ gespeichert werden soll.</span><span class="sxs-lookup"><span data-stu-id="86403-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="86403-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="86403-136">redirectTo</span></span> | <span data-ttu-id="86403-137">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="86403-137">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="86403-138">Die e-Mail-Adressen in denen eine Nachricht umgeleitet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="86403-138">The email addresses to which a message should be redirected.</span></span> |
| <span data-ttu-id="86403-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="86403-139">stopProcessingRules</span></span> | <span data-ttu-id="86403-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86403-140">Boolean</span></span> | <span data-ttu-id="86403-141">Gibt an, ob nachfolgende Regeln ausgewertet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="86403-141">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="86403-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="86403-142">JSON representation</span></span>
<span data-ttu-id="86403-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="86403-143">Here is a JSON representation of the resource.</span></span>

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
