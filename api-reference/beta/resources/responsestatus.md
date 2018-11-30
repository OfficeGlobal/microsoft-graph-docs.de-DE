---
title: responseStatus-Ressourcentyp
description: Der Antwortstatus einer Besprechungsanfrage.
ms.openlocfilehash: 9a6ddb26f018535682611152a69c2039f1c7f016
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061211"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="da1ec-103">responseStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="da1ec-103">responseStatus resource type</span></span>

> <span data-ttu-id="da1ec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="da1ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da1ec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da1ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da1ec-106">Der Antwortstatus einer Besprechungsanfrage.</span><span class="sxs-lookup"><span data-stu-id="da1ec-106">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="da1ec-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="da1ec-107">Properties</span></span>

| <span data-ttu-id="da1ec-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da1ec-108">Property</span></span> | <span data-ttu-id="da1ec-109">Typ</span><span class="sxs-lookup"><span data-stu-id="da1ec-109">Type</span></span>           | <span data-ttu-id="da1ec-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da1ec-110">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="da1ec-111">Antwort</span><span class="sxs-lookup"><span data-stu-id="da1ec-111">response</span></span> | <span data-ttu-id="da1ec-112">String</span><span class="sxs-lookup"><span data-stu-id="da1ec-112">String</span></span>         | <span data-ttu-id="da1ec-113">Der Antworttyp.</span><span class="sxs-lookup"><span data-stu-id="da1ec-113">The response type.</span></span> <span data-ttu-id="da1ec-114">Mögliche Werte: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="da1ec-114">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="da1ec-115">Uhrzeit</span><span class="sxs-lookup"><span data-stu-id="da1ec-115">time</span></span>     | <span data-ttu-id="da1ec-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da1ec-116">DateTimeOffset</span></span> | <span data-ttu-id="da1ec-p103">Datum und Uhrzeit, an dem bzw. der die Antwort zurückgegeben wurde. Hierfür wird das ISO 8601-Format, und die Angabe erfolgt immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="da1ec-p103">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="da1ec-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="da1ec-120">JSON representation</span></span>

<span data-ttu-id="da1ec-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="da1ec-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
