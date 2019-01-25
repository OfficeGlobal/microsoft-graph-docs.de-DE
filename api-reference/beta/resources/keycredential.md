---
title: Ressourcentyp keyCredential
description: Enthält eine wichtige Anmeldeinformationen eine Anwendung oder einen Dienstprinzipal zugeordnet ist. Die **KeyCredentials** -Eigenschaft der Anwendung und ServicePrincipal Entitäten ist eine Auflistung von **KeyCredential**.
localization_priority: Normal
ms.openlocfilehash: 87223ab77bc18ca57fb2bd9635cd0790f0651fb7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519052"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="a89ad-104">Ressourcentyp keyCredential</span><span class="sxs-lookup"><span data-stu-id="a89ad-104">keyCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a89ad-105">Enthält eine wichtige Anmeldeinformationen eine Anwendung oder einen Dienstprinzipal zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="a89ad-105">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="a89ad-106">Die **KeyCredentials** -Eigenschaft der [Anwendung](application.md) und [ServicePrincipal](serviceprincipal.md) Entitäten ist eine Auflistung von **KeyCredential**.</span><span class="sxs-lookup"><span data-stu-id="a89ad-106">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a89ad-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a89ad-107">JSON representation</span></span>

<span data-ttu-id="a89ad-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a89ad-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a><span data-ttu-id="a89ad-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a89ad-109">Properties</span></span>
| <span data-ttu-id="a89ad-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a89ad-110">Property</span></span>     | <span data-ttu-id="a89ad-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a89ad-111">Type</span></span>   |<span data-ttu-id="a89ad-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a89ad-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a89ad-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="a89ad-113">customKeyIdentifier</span></span>|<span data-ttu-id="a89ad-114">Binär</span><span class="sxs-lookup"><span data-stu-id="a89ad-114">Binary</span></span>| <span data-ttu-id="a89ad-115">Benutzerdefinierte Schlüssel-ID</span><span class="sxs-lookup"><span data-stu-id="a89ad-115">Custom key identifier</span></span> |
|<span data-ttu-id="a89ad-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a89ad-116">endDateTime</span></span>|<span data-ttu-id="a89ad-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a89ad-117">DateTimeOffset</span></span>|<span data-ttu-id="a89ad-118">Datum und Uhrzeit, zu der die Anmeldeinformationen abläuft. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="a89ad-118">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a89ad-119">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a89ad-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a89ad-120">Schlüssel-ID</span><span class="sxs-lookup"><span data-stu-id="a89ad-120">keyId</span></span>|<span data-ttu-id="a89ad-121">Guid</span><span class="sxs-lookup"><span data-stu-id="a89ad-121">Guid</span></span>|<span data-ttu-id="a89ad-122">Der eindeutige Bezeichner (GUID) für den Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="a89ad-122">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="a89ad-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a89ad-123">startDateTime</span></span>|<span data-ttu-id="a89ad-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a89ad-124">DateTimeOffset</span></span>|<span data-ttu-id="a89ad-125">Datum und Uhrzeit, an dem die Anmeldeinformationen gültig ist. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="a89ad-125">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a89ad-126">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a89ad-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a89ad-127">type</span><span class="sxs-lookup"><span data-stu-id="a89ad-127">type</span></span>|<span data-ttu-id="a89ad-128">String</span><span class="sxs-lookup"><span data-stu-id="a89ad-128">String</span></span>|<span data-ttu-id="a89ad-129">Die Art der wichtigsten Anmeldeinformationen. beispielsweise "Symmetrisch".</span><span class="sxs-lookup"><span data-stu-id="a89ad-129">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="a89ad-130">Verwendung</span><span class="sxs-lookup"><span data-stu-id="a89ad-130">usage</span></span>|<span data-ttu-id="a89ad-131">String</span><span class="sxs-lookup"><span data-stu-id="a89ad-131">String</span></span>|<span data-ttu-id="a89ad-132">Eine Zeichenfolge, die den Zweck beschreibt, für den der Schlüssel verwendet werden kann. beispielsweise "Überprüfen".</span><span class="sxs-lookup"><span data-stu-id="a89ad-132">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="a89ad-133">Key</span><span class="sxs-lookup"><span data-stu-id="a89ad-133">key</span></span>|<span data-ttu-id="a89ad-134">Binär</span><span class="sxs-lookup"><span data-stu-id="a89ad-134">Binary</span></span>|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/keycredential.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
