---
title: Ressourcentyp tokenMeetingInfo
description: Der Typ des TokenMeetingInfo.
author: VinodRavichandran
ms.openlocfilehash: 6fa66fef6f401db848a9ed3e92c5a1003a5294b6
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380548"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="a914d-103">Ressourcentyp tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="a914d-103">tokenMeetingInfo resource type</span></span>

> <span data-ttu-id="a914d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a914d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a914d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a914d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a914d-106">Der Typ des TokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="a914d-106">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="a914d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a914d-107">Properties</span></span>

| <span data-ttu-id="a914d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a914d-108">Property</span></span>                     | <span data-ttu-id="a914d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a914d-109">Type</span></span>    | <span data-ttu-id="a914d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a914d-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="a914d-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="a914d-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="a914d-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a914d-112">Boolean</span></span> | <span data-ttu-id="a914d-113">Gibt an, ob eine Unterhaltung fortgesetzt werden kann, sobald der Host der Unterhaltung verlässt.</span><span class="sxs-lookup"><span data-stu-id="a914d-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="a914d-114">token</span><span class="sxs-lookup"><span data-stu-id="a914d-114">token</span></span>                        | <span data-ttu-id="a914d-115">String</span><span class="sxs-lookup"><span data-stu-id="a914d-115">String</span></span>  | <span data-ttu-id="a914d-116">Das Token an der Besprechung teilnehmen/aktivieren.</span><span class="sxs-lookup"><span data-stu-id="a914d-116">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="a914d-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a914d-117">JSON representation</span></span>

<span data-ttu-id="a914d-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a914d-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="a914d-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a914d-119">Example</span></span>

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
