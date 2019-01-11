---
title: Ressourcentyp tokenMeetingInfo
description: Der Typ des TokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9a618906df450ce58f7428a76367e896b315591a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806979"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="182f4-103">Ressourcentyp tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="182f4-103">tokenMeetingInfo resource type</span></span>

> <span data-ttu-id="182f4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="182f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="182f4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="182f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="182f4-106">Der Typ des TokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="182f4-106">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="182f4-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="182f4-107">Properties</span></span>

| <span data-ttu-id="182f4-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="182f4-108">Property</span></span>                     | <span data-ttu-id="182f4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="182f4-109">Type</span></span>    | <span data-ttu-id="182f4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="182f4-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="182f4-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="182f4-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="182f4-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="182f4-112">Boolean</span></span> | <span data-ttu-id="182f4-113">Gibt an, ob eine Unterhaltung fortgesetzt werden kann, sobald der Host der Unterhaltung verlässt.</span><span class="sxs-lookup"><span data-stu-id="182f4-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="182f4-114">token</span><span class="sxs-lookup"><span data-stu-id="182f4-114">token</span></span>                        | <span data-ttu-id="182f4-115">String</span><span class="sxs-lookup"><span data-stu-id="182f4-115">String</span></span>  | <span data-ttu-id="182f4-116">Das Token an der Besprechung teilnehmen/aktivieren.</span><span class="sxs-lookup"><span data-stu-id="182f4-116">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="182f4-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="182f4-117">JSON representation</span></span>

<span data-ttu-id="182f4-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="182f4-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="182f4-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="182f4-119">Example</span></span>

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
