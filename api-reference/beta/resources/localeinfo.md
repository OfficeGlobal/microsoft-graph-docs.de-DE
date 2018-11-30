---
title: localeInfo-Ressourcentyp
description: Die Gebietsschemainformationen, einschließlich der bevorzugten Sprache und Land/Region, des angemeldeten Benutzers.
ms.openlocfilehash: 5dae464a4931fb094ae47cce600a95d55c6c3f93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064465"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="0f278-103">localeInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0f278-103">localeInfo resource type</span></span>

> <span data-ttu-id="0f278-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0f278-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f278-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f278-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f278-106">Die Gebietsschemainformationen, einschließlich der bevorzugten Sprache und Land/Region, des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="0f278-106">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="0f278-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f278-107">Properties</span></span>
| <span data-ttu-id="0f278-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f278-108">Property</span></span>     | <span data-ttu-id="0f278-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0f278-109">Type</span></span>   |<span data-ttu-id="0f278-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f278-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f278-111">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="0f278-111">locale</span></span>|<span data-ttu-id="0f278-112">string</span><span class="sxs-lookup"><span data-stu-id="0f278-112">string</span></span>|<span data-ttu-id="0f278-p102">Eine Gebietsschemadarstellung für den Benutzer, die die bevorzugte Sprache des Benutzers sowie Land/Region umfasst. Z. B. „de-de“. Die Sprachkomponente besteht entsprechend der Definitionen in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm) aus 2 Buchstaben, und die Länderkomponente besteht entsprechend der Definitionen in [ISO 3166-1-Alpha-2](https://www.iso.org/iso/country_codes.htm) aus 2 Buchstaben.</span><span class="sxs-lookup"><span data-stu-id="0f278-p102">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="0f278-116">displayName</span><span class="sxs-lookup"><span data-stu-id="0f278-116">displayName</span></span>|<span data-ttu-id="0f278-117">string</span><span class="sxs-lookup"><span data-stu-id="0f278-117">string</span></span>|<span data-ttu-id="0f278-118">Ein Name, der das Gebietsschema des Benutzers in natürlicher Sprache darstellt, z. B. „Englisch (USA)“.</span><span class="sxs-lookup"><span data-stu-id="0f278-118">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f278-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f278-119">JSON representation</span></span>

<span data-ttu-id="0f278-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f278-120">Here is a JSON representation of the resource.</span></span>

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