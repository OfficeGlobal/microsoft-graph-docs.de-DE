---
title: Ressourcentyp agreementAcceptance
description: Den aktuellen Status der ein Benutzer innerhalb eines Unternehmens anpassbare rechtliche Hinweise von Azure Active Directory (AD Azure) basiertes Bereichs darstellt.
localization_priority: Normal
ms.openlocfilehash: 884a6b7dcf4dcc8f00aa927dd9d486c074b64183
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518870"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="ed78c-103">Ressourcentyp agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="ed78c-103">agreementAcceptance resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed78c-104">Den aktuellen Status der ein Benutzer innerhalb eines Unternehmens anpassbare rechtliche Hinweise von Azure Active Directory (AD Azure) basiertes Bereichs darstellt.</span><span class="sxs-lookup"><span data-stu-id="ed78c-104">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="ed78c-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ed78c-105">Properties</span></span>
| <span data-ttu-id="ed78c-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed78c-106">Property</span></span>     | <span data-ttu-id="ed78c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="ed78c-107">Type</span></span>        | <span data-ttu-id="ed78c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed78c-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ed78c-109">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="ed78c-109">agreementFileId</span></span>|<span data-ttu-id="ed78c-110">String</span><span class="sxs-lookup"><span data-stu-id="ed78c-110">String</span></span>|<span data-ttu-id="ed78c-111">Die ID der Vereinbarung-Datei, die vom Benutzer angenommen.</span><span class="sxs-lookup"><span data-stu-id="ed78c-111">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="ed78c-112">agreementId</span><span class="sxs-lookup"><span data-stu-id="ed78c-112">agreementId</span></span>|<span data-ttu-id="ed78c-113">String</span><span class="sxs-lookup"><span data-stu-id="ed78c-113">String</span></span>|<span data-ttu-id="ed78c-114">ID des zu.</span><span class="sxs-lookup"><span data-stu-id="ed78c-114">ID of the agreement.</span></span>|
|<span data-ttu-id="ed78c-115">id</span><span class="sxs-lookup"><span data-stu-id="ed78c-115">id</span></span>|<span data-ttu-id="ed78c-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ed78c-116">String</span></span>| <span data-ttu-id="ed78c-117">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed78c-117">Read-only.</span></span>|
|<span data-ttu-id="ed78c-118">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed78c-118">recordedDateTime</span></span>|<span data-ttu-id="ed78c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed78c-119">DateTimeOffset</span></span>|<span data-ttu-id="ed78c-p101">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ed78c-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ed78c-122">state</span><span class="sxs-lookup"><span data-stu-id="ed78c-122">state</span></span>|<span data-ttu-id="ed78c-123">string</span><span class="sxs-lookup"><span data-stu-id="ed78c-123">string</span></span>| <span data-ttu-id="ed78c-124">Mögliche Werte sind: `accepted` und `declined`.</span><span class="sxs-lookup"><span data-stu-id="ed78c-124">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="ed78c-125">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ed78c-125">userDisplayName</span></span>|<span data-ttu-id="ed78c-126">String</span><span class="sxs-lookup"><span data-stu-id="ed78c-126">String</span></span>|<span data-ttu-id="ed78c-127">Der Anzeigename des Benutzers, wenn die Annahme aufgezeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="ed78c-127">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="ed78c-128">userEmail</span><span class="sxs-lookup"><span data-stu-id="ed78c-128">userEmail</span></span>|<span data-ttu-id="ed78c-129">String</span><span class="sxs-lookup"><span data-stu-id="ed78c-129">String</span></span>|<span data-ttu-id="ed78c-130">E-Mail des Benutzers, wenn die Annahme aufgezeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="ed78c-130">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="ed78c-131">userId</span><span class="sxs-lookup"><span data-stu-id="ed78c-131">userId</span></span>|<span data-ttu-id="ed78c-132">String</span><span class="sxs-lookup"><span data-stu-id="ed78c-132">String</span></span>|<span data-ttu-id="ed78c-133">ID des Benutzers, der den Lizenzvertrag akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="ed78c-133">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="ed78c-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ed78c-134">userPrincipalName</span></span>|<span data-ttu-id="ed78c-135">String</span><span class="sxs-lookup"><span data-stu-id="ed78c-135">String</span></span>|<span data-ttu-id="ed78c-136">UPN des Benutzers, wenn die Annahme aufgezeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="ed78c-136">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed78c-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ed78c-137">Relationships</span></span>
<span data-ttu-id="ed78c-138">Keine</span><span class="sxs-lookup"><span data-stu-id="ed78c-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ed78c-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ed78c-139">JSON representation</span></span>

<span data-ttu-id="ed78c-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ed78c-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
  "agreementFileId": "String",
  "agreementId": "String",
  "id": "String (identifier)",
  "recordedDateTime": "String (timestamp)",
  "state": "string",
  "userDisplayName": "String",
  "userEmail": "String",
  "userId": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementacceptance.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
