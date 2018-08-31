# <a name="messageruleactions-resource-type"></a><span data-ttu-id="8e351-101">messageRuleActions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8e351-101">messageRuleActions resource type</span></span>


<span data-ttu-id="8e351-102">Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="8e351-102">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="8e351-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8e351-103">Properties</span></span>
| <span data-ttu-id="8e351-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e351-104">Property</span></span>     | <span data-ttu-id="8e351-105">Typ</span><span class="sxs-lookup"><span data-stu-id="8e351-105">Type</span></span>   |<span data-ttu-id="8e351-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e351-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8e351-107">assignCategories</span><span class="sxs-lookup"><span data-stu-id="8e351-107">assignCategories</span></span> | <span data-ttu-id="8e351-108">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="8e351-108">String collection</span></span> | <span data-ttu-id="8e351-109">Eine Liste von Kategorien, die einer Nachricht zugewiesen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8e351-109">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="8e351-110">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="8e351-110">copyToFolder</span></span> | <span data-ttu-id="8e351-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e351-111">String</span></span> | <span data-ttu-id="8e351-112">Die ID eines Ordners, in den eine Nachricht kopiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="8e351-112">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="8e351-113">Löschen</span><span class="sxs-lookup"><span data-stu-id="8e351-113">delete</span></span> | <span data-ttu-id="8e351-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e351-114">Boolean</span></span> | <span data-ttu-id="8e351-115">Gibt an, ob eine Nachricht in den Ordner „Gelöschte Elemente“ verschoben werden soll.</span><span class="sxs-lookup"><span data-stu-id="8e351-115">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="8e351-116">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="8e351-116">forwardAsAttachmentTo</span></span> | <span data-ttu-id="8e351-117">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8e351-117">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="8e351-118">Die E-Mail-Adressen der Empfänger, an die eine Nachricht als Anlage weitergeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8e351-118">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="8e351-119">forwardTo</span><span class="sxs-lookup"><span data-stu-id="8e351-119">forwardTo</span></span> | <span data-ttu-id="8e351-120">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8e351-120">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="8e351-121">Die E-Mail-Adressen der Empfänger, an die eine Nachricht weitergeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8e351-121">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="8e351-122">markAsRead</span><span class="sxs-lookup"><span data-stu-id="8e351-122">markAsRead</span></span> | <span data-ttu-id="8e351-123">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e351-123">Boolean</span></span> | <span data-ttu-id="8e351-124">Gibt an, ob eine Nachricht als gelesen markiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="8e351-124">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="8e351-125">markImportance</span><span class="sxs-lookup"><span data-stu-id="8e351-125">markImportance</span></span> | <span data-ttu-id="8e351-126">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="8e351-126">importance</span></span> | <span data-ttu-id="8e351-127">Legt die Wichtigkeit der Nachricht fest. Die folgenden Einstellungen sind möglich: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8e351-127">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="8e351-128">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="8e351-128">moveToFolder</span></span> |  <span data-ttu-id="8e351-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e351-129">String</span></span>| <span data-ttu-id="8e351-130">Die ID des Ordners, in den eine Nachricht verschoben wird.</span><span class="sxs-lookup"><span data-stu-id="8e351-130">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="8e351-131">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="8e351-131">permanentDelete</span></span> | <span data-ttu-id="8e351-132">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e351-132">Boolean</span></span> | <span data-ttu-id="8e351-133">Gibt an, ob eine Nachricht dauerhaft gelöscht und nicht im Ordner „Gelöschte Elemente“ gespeichert werden soll.</span><span class="sxs-lookup"><span data-stu-id="8e351-133">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="8e351-134">redirectTo</span><span class="sxs-lookup"><span data-stu-id="8e351-134">redirectTo</span></span> | <span data-ttu-id="8e351-135">[Empfänger](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8e351-135">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="8e351-136">Die E-Mail-Adresse, an die eine Nachricht umgeleitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8e351-136">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="8e351-137">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="8e351-137">stopProcessingRules</span></span> | <span data-ttu-id="8e351-138">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e351-138">Boolean</span></span> | <span data-ttu-id="8e351-139">Gibt an, ob nachfolgende Regeln ausgewertet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8e351-139">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8e351-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8e351-140">JSON representation</span></span>
<span data-ttu-id="8e351-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8e351-141">Here is a JSON representation of the resource.</span></span>

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