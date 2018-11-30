---
title: Ressourcentyp chatMessageMention
description: 'Stellt einen Vermerk in einer ChatMessage Entität dar. Benutzer, Team, Bot oder DDE-Kanal kann die Erwähnung sein. '
ms.openlocfilehash: 5f1e427b0ed2b8ffcfbc86417beb4719dc6fb2a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058431"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="9dcda-104">Ressourcentyp chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="9dcda-104">chatMessageMention resource type</span></span>

> <span data-ttu-id="9dcda-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9dcda-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9dcda-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9dcda-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9dcda-107">Stellt einen Vermerk in einer [ChatMessage](chatmessage.md) Entität dar.</span><span class="sxs-lookup"><span data-stu-id="9dcda-107">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="9dcda-108">Benutzer, Team, Bot oder DDE-Kanal kann die Erwähnung sein.</span><span class="sxs-lookup"><span data-stu-id="9dcda-108">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="9dcda-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9dcda-109">Properties</span></span>
| <span data-ttu-id="9dcda-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9dcda-110">Property</span></span>     | <span data-ttu-id="9dcda-111">Typ</span><span class="sxs-lookup"><span data-stu-id="9dcda-111">Type</span></span>   |<span data-ttu-id="9dcda-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dcda-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dcda-113">id</span><span class="sxs-lookup"><span data-stu-id="9dcda-113">id</span></span>|<span data-ttu-id="9dcda-114">string</span><span class="sxs-lookup"><span data-stu-id="9dcda-114">string</span></span>|<span data-ttu-id="9dcda-115">ID der Entität erwähnt wird</span><span class="sxs-lookup"><span data-stu-id="9dcda-115">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="9dcda-116">mentionText</span><span class="sxs-lookup"><span data-stu-id="9dcda-116">mentionText</span></span>|<span data-ttu-id="9dcda-117">string</span><span class="sxs-lookup"><span data-stu-id="9dcda-117">string</span></span>|<span data-ttu-id="9dcda-118">Zeichenfolge, mit der Erwähnung Ex dargestellt: Anzeigename des Benutzers, Teamname usw.</span><span class="sxs-lookup"><span data-stu-id="9dcda-118">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="9dcda-119">erwähnten</span><span class="sxs-lookup"><span data-stu-id="9dcda-119">mentioned</span></span>|[<span data-ttu-id="9dcda-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="9dcda-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="9dcda-121">Der Benutzer, der erwähnt wurde</span><span class="sxs-lookup"><span data-stu-id="9dcda-121">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9dcda-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9dcda-122">JSON representation</span></span>

<span data-ttu-id="9dcda-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9dcda-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
