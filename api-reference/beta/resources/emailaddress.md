---
title: emailAddress-Ressourcentyp
description: Stellt den Namen und die SMTP-Adresse einer Instanz einer Entität, beispielsweise eine Nachricht Empfänger oder Kalender Besitzer.
localization_priority: Normal
ms.openlocfilehash: 5286334378aa5d208cf171ecab0bdc1777a4073b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871225"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="85b62-103">emailAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="85b62-103">emailAddress resource type</span></span>

> <span data-ttu-id="85b62-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="85b62-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85b62-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85b62-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85b62-106">Stellt den Namen und die SMTP-Adresse einer Instanz einer Entität, beispielsweise eine Nachricht Empfänger oder Kalender Besitzer.</span><span class="sxs-lookup"><span data-stu-id="85b62-106">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="85b62-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="85b62-107">Properties</span></span>
| <span data-ttu-id="85b62-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85b62-108">Property</span></span>     | <span data-ttu-id="85b62-109">Typ</span><span class="sxs-lookup"><span data-stu-id="85b62-109">Type</span></span>   |<span data-ttu-id="85b62-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85b62-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85b62-111">address</span><span class="sxs-lookup"><span data-stu-id="85b62-111">address</span></span>|<span data-ttu-id="85b62-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85b62-112">String</span></span>|<span data-ttu-id="85b62-113">Die e-Mail-Adresse einer Instanz einer Entität.</span><span class="sxs-lookup"><span data-stu-id="85b62-113">The email address of an entity instance.</span></span>|
|<span data-ttu-id="85b62-114">name</span><span class="sxs-lookup"><span data-stu-id="85b62-114">name</span></span>|<span data-ttu-id="85b62-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85b62-115">String</span></span>|<span data-ttu-id="85b62-116">Der Anzeigename einer Instanz einer Entität.</span><span class="sxs-lookup"><span data-stu-id="85b62-116">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85b62-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="85b62-117">JSON representation</span></span>

<span data-ttu-id="85b62-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="85b62-118">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
