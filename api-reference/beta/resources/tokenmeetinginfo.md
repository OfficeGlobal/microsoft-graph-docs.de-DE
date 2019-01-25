---
title: Ressourcentyp tokenMeetingInfo
description: Der Typ des TokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8e115887e67f19375ca8b96a216af98c80e0b312
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513368"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="3ff03-103">Ressourcentyp tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="3ff03-103">tokenMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ff03-104">Der Typ des TokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="3ff03-104">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="3ff03-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3ff03-105">Properties</span></span>

| <span data-ttu-id="3ff03-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ff03-106">Property</span></span>                     | <span data-ttu-id="3ff03-107">Typ</span><span class="sxs-lookup"><span data-stu-id="3ff03-107">Type</span></span>    | <span data-ttu-id="3ff03-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ff03-108">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="3ff03-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="3ff03-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="3ff03-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3ff03-110">Boolean</span></span> | <span data-ttu-id="3ff03-111">Gibt an, ob eine Unterhaltung fortgesetzt werden kann, sobald der Host der Unterhaltung verlässt.</span><span class="sxs-lookup"><span data-stu-id="3ff03-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="3ff03-112">token</span><span class="sxs-lookup"><span data-stu-id="3ff03-112">token</span></span>                        | <span data-ttu-id="3ff03-113">String</span><span class="sxs-lookup"><span data-stu-id="3ff03-113">String</span></span>  | <span data-ttu-id="3ff03-114">Das Token an der Besprechung teilnehmen/aktivieren.</span><span class="sxs-lookup"><span data-stu-id="3ff03-114">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="3ff03-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3ff03-115">JSON representation</span></span>

<span data-ttu-id="3ff03-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3ff03-116">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="3ff03-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ff03-117">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tokenmeetinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
