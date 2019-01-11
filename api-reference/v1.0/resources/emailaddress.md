---
title: emailAddress-Ressourcentyp
description: Name und E-Mail-Adresse eines Kontakts oder eines Empfängers der Nachricht.
localization_priority: Normal
ms.openlocfilehash: 5ea1919e5c5f389c9b7fece508e8339f722b725a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826884"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="9e9fc-103">emailAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9e9fc-103">emailAddress resource type</span></span>

<span data-ttu-id="9e9fc-104">Name und E-Mail-Adresse eines Kontakts oder eines Empfängers der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="9e9fc-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="9e9fc-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e9fc-105">Properties</span></span>
| <span data-ttu-id="9e9fc-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e9fc-106">Property</span></span>     | <span data-ttu-id="9e9fc-107">Typ</span><span class="sxs-lookup"><span data-stu-id="9e9fc-107">Type</span></span>   |<span data-ttu-id="9e9fc-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e9fc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e9fc-109">address</span><span class="sxs-lookup"><span data-stu-id="9e9fc-109">address</span></span>|<span data-ttu-id="9e9fc-110">String</span><span class="sxs-lookup"><span data-stu-id="9e9fc-110">String</span></span>|<span data-ttu-id="9e9fc-111">Die E-Mail-Adresse der Person oder Organisation.</span><span class="sxs-lookup"><span data-stu-id="9e9fc-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="9e9fc-112">name</span><span class="sxs-lookup"><span data-stu-id="9e9fc-112">name</span></span>|<span data-ttu-id="9e9fc-113">String</span><span class="sxs-lookup"><span data-stu-id="9e9fc-113">String</span></span>|<span data-ttu-id="9e9fc-114">Der Anzeigename der Person oder Entität.</span><span class="sxs-lookup"><span data-stu-id="9e9fc-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e9fc-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e9fc-115">JSON representation</span></span>

<span data-ttu-id="9e9fc-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e9fc-116">Here is a JSON representation of the resource</span></span>

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
