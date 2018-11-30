---
title: Ressourcentyp keyCredential
description: Enthält eine wichtige Anmeldeinformationen eine Anwendung oder einen Dienstprinzipal zugeordnet ist. Die **KeyCredentials** -Eigenschaft der Anwendung und ServicePrincipal Entitäten ist eine Auflistung von **KeyCredential**.
ms.openlocfilehash: d4509360c0425c255566b9f77b9ecd96cf349dec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058460"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="374f7-104">Ressourcentyp keyCredential</span><span class="sxs-lookup"><span data-stu-id="374f7-104">keyCredential resource type</span></span>

> <span data-ttu-id="374f7-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="374f7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="374f7-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="374f7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="374f7-107">Enthält eine wichtige Anmeldeinformationen eine Anwendung oder einen Dienstprinzipal zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="374f7-107">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="374f7-108">Die **KeyCredentials** -Eigenschaft der [Anwendung](application.md) und [ServicePrincipal](serviceprincipal.md) Entitäten ist eine Auflistung von **KeyCredential**.</span><span class="sxs-lookup"><span data-stu-id="374f7-108">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="374f7-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="374f7-109">JSON representation</span></span>

<span data-ttu-id="374f7-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="374f7-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="374f7-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="374f7-111">Properties</span></span>
| <span data-ttu-id="374f7-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="374f7-112">Property</span></span>     | <span data-ttu-id="374f7-113">Typ</span><span class="sxs-lookup"><span data-stu-id="374f7-113">Type</span></span>   |<span data-ttu-id="374f7-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="374f7-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="374f7-115">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="374f7-115">customKeyIdentifier</span></span>|<span data-ttu-id="374f7-116">Binär</span><span class="sxs-lookup"><span data-stu-id="374f7-116">Binary</span></span>| <span data-ttu-id="374f7-117">Benutzerdefinierte Schlüssel-ID</span><span class="sxs-lookup"><span data-stu-id="374f7-117">Custom key identifier</span></span> |
|<span data-ttu-id="374f7-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="374f7-118">endDateTime</span></span>|<span data-ttu-id="374f7-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="374f7-119">DateTimeOffset</span></span>|<span data-ttu-id="374f7-120">Datum und Uhrzeit, zu der die Anmeldeinformationen abläuft. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="374f7-120">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="374f7-121">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="374f7-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="374f7-122">Schlüssel-ID</span><span class="sxs-lookup"><span data-stu-id="374f7-122">keyId</span></span>|<span data-ttu-id="374f7-123">Guid</span><span class="sxs-lookup"><span data-stu-id="374f7-123">Guid</span></span>|<span data-ttu-id="374f7-124">Der eindeutige Bezeichner (GUID) für den Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="374f7-124">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="374f7-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="374f7-125">startDateTime</span></span>|<span data-ttu-id="374f7-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="374f7-126">DateTimeOffset</span></span>|<span data-ttu-id="374f7-127">Datum und Uhrzeit, an dem die Anmeldeinformationen gültig ist. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="374f7-127">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="374f7-128">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="374f7-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="374f7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="374f7-129">type</span></span>|<span data-ttu-id="374f7-130">String</span><span class="sxs-lookup"><span data-stu-id="374f7-130">String</span></span>|<span data-ttu-id="374f7-131">Die Art der wichtigsten Anmeldeinformationen. beispielsweise "Symmetrisch".</span><span class="sxs-lookup"><span data-stu-id="374f7-131">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="374f7-132">Verwendung</span><span class="sxs-lookup"><span data-stu-id="374f7-132">usage</span></span>|<span data-ttu-id="374f7-133">String</span><span class="sxs-lookup"><span data-stu-id="374f7-133">String</span></span>|<span data-ttu-id="374f7-134">Eine Zeichenfolge, die den Zweck beschreibt, für den der Schlüssel verwendet werden kann. beispielsweise "Überprüfen".</span><span class="sxs-lookup"><span data-stu-id="374f7-134">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="374f7-135">Key</span><span class="sxs-lookup"><span data-stu-id="374f7-135">key</span></span>|<span data-ttu-id="374f7-136">Binär</span><span class="sxs-lookup"><span data-stu-id="374f7-136">Binary</span></span>|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->