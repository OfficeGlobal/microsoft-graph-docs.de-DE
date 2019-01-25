---
title: Ressourcentyp chatMessageMention
description: 'Stellt einen Vermerk in einer ChatMessage Entität dar. Benutzer, Team, Bot oder DDE-Kanal kann die Erwähnung sein. '
localization_priority: Normal
ms.openlocfilehash: f37374a9793000ba641ed772e5dbfca5c0f1bd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515349"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="fe5bc-104">Ressourcentyp chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="fe5bc-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe5bc-105">Stellt einen Vermerk in einer [ChatMessage](chatmessage.md) Entität dar.</span><span class="sxs-lookup"><span data-stu-id="fe5bc-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="fe5bc-106">Benutzer, Team, Bot oder DDE-Kanal kann die Erwähnung sein.</span><span class="sxs-lookup"><span data-stu-id="fe5bc-106">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="fe5bc-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fe5bc-107">Properties</span></span>
| <span data-ttu-id="fe5bc-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fe5bc-108">Property</span></span>     | <span data-ttu-id="fe5bc-109">Typ</span><span class="sxs-lookup"><span data-stu-id="fe5bc-109">Type</span></span>   |<span data-ttu-id="fe5bc-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe5bc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe5bc-111">id</span><span class="sxs-lookup"><span data-stu-id="fe5bc-111">id</span></span>|<span data-ttu-id="fe5bc-112">string</span><span class="sxs-lookup"><span data-stu-id="fe5bc-112">string</span></span>|<span data-ttu-id="fe5bc-113">ID der Entität erwähnt wird</span><span class="sxs-lookup"><span data-stu-id="fe5bc-113">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="fe5bc-114">mentionText</span><span class="sxs-lookup"><span data-stu-id="fe5bc-114">mentionText</span></span>|<span data-ttu-id="fe5bc-115">string</span><span class="sxs-lookup"><span data-stu-id="fe5bc-115">string</span></span>|<span data-ttu-id="fe5bc-116">Zeichenfolge, mit der Erwähnung Ex dargestellt: Anzeigename des Benutzers, Teamname usw.</span><span class="sxs-lookup"><span data-stu-id="fe5bc-116">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="fe5bc-117">erwähnten</span><span class="sxs-lookup"><span data-stu-id="fe5bc-117">mentioned</span></span>|[<span data-ttu-id="fe5bc-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="fe5bc-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="fe5bc-119">Der Benutzer, der erwähnt wurde</span><span class="sxs-lookup"><span data-stu-id="fe5bc-119">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe5bc-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fe5bc-120">JSON representation</span></span>

<span data-ttu-id="fe5bc-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fe5bc-121">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatMention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
