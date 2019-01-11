---
title: PasswordCredential Ressourcentyp
description: Eine Anwendung oder ein Dienst Prinzipal zugeordnete Kennwort Anmeldeinformationen enthält. Die **PasswordCredentials** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **PasswordCredential**.
localization_priority: Normal
ms.openlocfilehash: 5cb995c00a7dcfcfb4bda331e24dcb4d732f04f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814441"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="adbb6-104">PasswordCredential Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="adbb6-104">passwordCredential resource type</span></span>

> <span data-ttu-id="adbb6-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="adbb6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adbb6-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="adbb6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="adbb6-107">Eine Anwendung oder ein Dienst Prinzipal zugeordnete Kennwort Anmeldeinformationen enthält.</span><span class="sxs-lookup"><span data-stu-id="adbb6-107">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="adbb6-108">Die **PasswordCredentials** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **PasswordCredential**.</span><span class="sxs-lookup"><span data-stu-id="adbb6-108">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="adbb6-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="adbb6-109">JSON representation</span></span>

<span data-ttu-id="adbb6-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="adbb6-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a><span data-ttu-id="adbb6-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="adbb6-111">Properties</span></span>
| <span data-ttu-id="adbb6-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="adbb6-112">Property</span></span>     | <span data-ttu-id="adbb6-113">Typ</span><span class="sxs-lookup"><span data-stu-id="adbb6-113">Type</span></span>   |<span data-ttu-id="adbb6-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="adbb6-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adbb6-115">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="adbb6-115">customKeyIdentifier</span></span>|<span data-ttu-id="adbb6-116">Binär</span><span class="sxs-lookup"><span data-stu-id="adbb6-116">Binary</span></span>|            |
|<span data-ttu-id="adbb6-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="adbb6-117">endDateTime</span></span>|<span data-ttu-id="adbb6-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adbb6-118">DateTimeOffset</span></span>|<span data-ttu-id="adbb6-119">Datum und Uhrzeit, an dem das Kennwort läuft ab. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="adbb6-119">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="adbb6-120">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="adbb6-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="adbb6-121">Schlüssel-ID</span><span class="sxs-lookup"><span data-stu-id="adbb6-121">keyId</span></span>|<span data-ttu-id="adbb6-122">Guid</span><span class="sxs-lookup"><span data-stu-id="adbb6-122">Guid</span></span>|            |
|<span data-ttu-id="adbb6-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="adbb6-123">startDateTime</span></span>|<span data-ttu-id="adbb6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adbb6-124">DateTimeOffset</span></span>|<span data-ttu-id="adbb6-125">Datum und Uhrzeit, an dem das Kennwort gültig ist. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="adbb6-125">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="adbb6-126">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="adbb6-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="adbb6-127">secretText</span><span class="sxs-lookup"><span data-stu-id="adbb6-127">secretText</span></span>|<span data-ttu-id="adbb6-128">String</span><span class="sxs-lookup"><span data-stu-id="adbb6-128">String</span></span>| <span data-ttu-id="adbb6-129">Die Kennwörter müssen 16-64 Zeichen lang sein.</span><span class="sxs-lookup"><span data-stu-id="adbb6-129">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="adbb6-130">Hinweis</span><span class="sxs-lookup"><span data-stu-id="adbb6-130">hint</span></span>|<span data-ttu-id="adbb6-131">String</span><span class="sxs-lookup"><span data-stu-id="adbb6-131">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
