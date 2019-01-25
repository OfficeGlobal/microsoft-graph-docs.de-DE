---
title: emailAddress-Ressourcentyp
description: Stellt den Namen und die SMTP-Adresse einer Instanz einer Entität, beispielsweise eine Nachricht Empfänger oder Kalender Besitzer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bc1f00ab09ac71f4f3cd9eb1aff8163a537ce257
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518667"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="46f97-103">emailAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="46f97-103">emailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46f97-104">Stellt den Namen und die SMTP-Adresse einer Instanz einer Entität, beispielsweise eine Nachricht Empfänger oder Kalender Besitzer.</span><span class="sxs-lookup"><span data-stu-id="46f97-104">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="46f97-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46f97-105">Properties</span></span>
| <span data-ttu-id="46f97-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46f97-106">Property</span></span>     | <span data-ttu-id="46f97-107">Typ</span><span class="sxs-lookup"><span data-stu-id="46f97-107">Type</span></span>   |<span data-ttu-id="46f97-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46f97-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46f97-109">address</span><span class="sxs-lookup"><span data-stu-id="46f97-109">address</span></span>|<span data-ttu-id="46f97-110">String</span><span class="sxs-lookup"><span data-stu-id="46f97-110">String</span></span>|<span data-ttu-id="46f97-111">Die e-Mail-Adresse einer Instanz einer Entität.</span><span class="sxs-lookup"><span data-stu-id="46f97-111">The email address of an entity instance.</span></span>|
|<span data-ttu-id="46f97-112">name</span><span class="sxs-lookup"><span data-stu-id="46f97-112">name</span></span>|<span data-ttu-id="46f97-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46f97-113">String</span></span>|<span data-ttu-id="46f97-114">Der Anzeigename einer Instanz einer Entität.</span><span class="sxs-lookup"><span data-stu-id="46f97-114">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46f97-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46f97-115">JSON representation</span></span>

<span data-ttu-id="46f97-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="46f97-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/emailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
