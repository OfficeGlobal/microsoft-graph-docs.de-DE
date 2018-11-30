---
title: Ressourcentyp tokenMeetingInfo
description: Der Typ des TokenMeetingInfo.
ms.openlocfilehash: ddaf9a0c36ce4a8a31c56e4db2e065ef186c4053
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059364"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="45346-103">Ressourcentyp tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="45346-103">tokenMeetingInfo resource type</span></span>

> <span data-ttu-id="45346-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="45346-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45346-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="45346-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45346-106">Der Typ des TokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="45346-106">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="45346-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="45346-107">Properties</span></span>

| <span data-ttu-id="45346-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="45346-108">Property</span></span>                     | <span data-ttu-id="45346-109">Typ</span><span class="sxs-lookup"><span data-stu-id="45346-109">Type</span></span>    | <span data-ttu-id="45346-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45346-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="45346-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="45346-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="45346-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="45346-112">Boolean</span></span> | <span data-ttu-id="45346-113">Gibt an, ob eine Unterhaltung fortgesetzt werden kann, sobald der Host der Unterhaltung verlässt.</span><span class="sxs-lookup"><span data-stu-id="45346-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="45346-114">token</span><span class="sxs-lookup"><span data-stu-id="45346-114">token</span></span>                        | <span data-ttu-id="45346-115">String</span><span class="sxs-lookup"><span data-stu-id="45346-115">String</span></span>  | <span data-ttu-id="45346-116">Das Token an der Besprechung teilnehmen/aktivieren.</span><span class="sxs-lookup"><span data-stu-id="45346-116">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="45346-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="45346-117">JSON representation</span></span>

<span data-ttu-id="45346-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="45346-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="45346-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45346-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
