---
title: PasswordCredential Ressourcentyp
description: Eine Anwendung oder ein Dienst Prinzipal zugeordnete Kennwort Anmeldeinformationen enthält. Die **PasswordCredentials** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **PasswordCredential**.
localization_priority: Normal
ms.openlocfilehash: 900bfb8a5828d636dfa1f1abfd0348ceb4aee143
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523148"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="0d527-104">PasswordCredential Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0d527-104">passwordCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d527-105">Eine Anwendung oder ein Dienst Prinzipal zugeordnete Kennwort Anmeldeinformationen enthält.</span><span class="sxs-lookup"><span data-stu-id="0d527-105">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="0d527-106">Die **PasswordCredentials** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **PasswordCredential**.</span><span class="sxs-lookup"><span data-stu-id="0d527-106">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0d527-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0d527-107">JSON representation</span></span>

<span data-ttu-id="0d527-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0d527-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="0d527-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0d527-109">Properties</span></span>
| <span data-ttu-id="0d527-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d527-110">Property</span></span>     | <span data-ttu-id="0d527-111">Typ</span><span class="sxs-lookup"><span data-stu-id="0d527-111">Type</span></span>   |<span data-ttu-id="0d527-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d527-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d527-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="0d527-113">customKeyIdentifier</span></span>|<span data-ttu-id="0d527-114">Binär</span><span class="sxs-lookup"><span data-stu-id="0d527-114">Binary</span></span>|            |
|<span data-ttu-id="0d527-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0d527-115">endDateTime</span></span>|<span data-ttu-id="0d527-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d527-116">DateTimeOffset</span></span>|<span data-ttu-id="0d527-117">Datum und Uhrzeit, an dem das Kennwort läuft ab. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="0d527-117">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0d527-118">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0d527-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0d527-119">Schlüssel-ID</span><span class="sxs-lookup"><span data-stu-id="0d527-119">keyId</span></span>|<span data-ttu-id="0d527-120">Guid</span><span class="sxs-lookup"><span data-stu-id="0d527-120">Guid</span></span>|            |
|<span data-ttu-id="0d527-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0d527-121">startDateTime</span></span>|<span data-ttu-id="0d527-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d527-122">DateTimeOffset</span></span>|<span data-ttu-id="0d527-123">Datum und Uhrzeit, an dem das Kennwort gültig ist. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="0d527-123">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0d527-124">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0d527-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0d527-125">secretText</span><span class="sxs-lookup"><span data-stu-id="0d527-125">secretText</span></span>|<span data-ttu-id="0d527-126">String</span><span class="sxs-lookup"><span data-stu-id="0d527-126">String</span></span>| <span data-ttu-id="0d527-127">Die Kennwörter müssen 16-64 Zeichen lang sein.</span><span class="sxs-lookup"><span data-stu-id="0d527-127">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="0d527-128">Hinweis</span><span class="sxs-lookup"><span data-stu-id="0d527-128">hint</span></span>|<span data-ttu-id="0d527-129">String</span><span class="sxs-lookup"><span data-stu-id="0d527-129">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/passwordcredential.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
