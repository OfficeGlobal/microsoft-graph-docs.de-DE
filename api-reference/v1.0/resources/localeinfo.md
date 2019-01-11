---
title: localeInfo-Ressourcentyp
description: Die Gebietsschemainformationen, einschließlich der bevorzugten Sprache und Land/Region, des angemeldeten Benutzers.
localization_priority: Normal
ms.openlocfilehash: 0c89a133ba31965b99099555ad18f185495fe4c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862587"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="f8a37-103">localeInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f8a37-103">localeInfo resource type</span></span>

<span data-ttu-id="f8a37-104">Die Gebietsschemainformationen, einschließlich der bevorzugten Sprache und Land/Region, des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f8a37-104">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="f8a37-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8a37-105">Properties</span></span>
| <span data-ttu-id="f8a37-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8a37-106">Property</span></span>     | <span data-ttu-id="f8a37-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f8a37-107">Type</span></span>   |<span data-ttu-id="f8a37-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8a37-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8a37-109">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="f8a37-109">locale</span></span>|<span data-ttu-id="f8a37-110">string</span><span class="sxs-lookup"><span data-stu-id="f8a37-110">string</span></span>|<span data-ttu-id="f8a37-p101">Eine Gebietsschemadarstellung für den Benutzer, die die bevorzugte Sprache des Benutzers sowie Land/Region umfasst. Z. B. „de-de“. Die Sprachkomponente besteht entsprechend der Definitionen in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm) aus 2 Buchstaben, und die Länderkomponente besteht entsprechend der Definitionen in [ISO 3166-1-Alpha-2](https://www.iso.org/iso/country_codes.htm) aus 2 Buchstaben.</span><span class="sxs-lookup"><span data-stu-id="f8a37-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="f8a37-114">displayName</span><span class="sxs-lookup"><span data-stu-id="f8a37-114">displayName</span></span>|<span data-ttu-id="f8a37-115">string</span><span class="sxs-lookup"><span data-stu-id="f8a37-115">string</span></span>|<span data-ttu-id="f8a37-116">Ein Name, der das Gebietsschema des Benutzers in natürlicher Sprache darstellt, z. B. „Englisch (USA)“.</span><span class="sxs-lookup"><span data-stu-id="f8a37-116">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8a37-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8a37-117">JSON representation</span></span>

<span data-ttu-id="f8a37-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8a37-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.localeInfo"
}-->

```json
{
  "locale": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
