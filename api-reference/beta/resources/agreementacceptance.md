---
title: Ressourcentyp agreementAcceptance
description: Den aktuellen Status der ein Benutzer innerhalb eines Unternehmens anpassbare rechtliche Hinweise von Azure Active Directory (AD Azure) basiertes Bereichs darstellt.
localization_priority: Normal
ms.openlocfilehash: b1c8a5e40fe6a12daf23566ae902ddf61f3ee4df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828282"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="e2ba6-103">Ressourcentyp agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="e2ba6-103">agreementAcceptance resource type</span></span>

> <span data-ttu-id="e2ba6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2ba6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2ba6-106">Den aktuellen Status der ein Benutzer innerhalb eines Unternehmens anpassbare rechtliche Hinweise von Azure Active Directory (AD Azure) basiertes Bereichs darstellt.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-106">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="e2ba6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e2ba6-107">Properties</span></span>
| <span data-ttu-id="e2ba6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2ba6-108">Property</span></span>     | <span data-ttu-id="e2ba6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e2ba6-109">Type</span></span>        | <span data-ttu-id="e2ba6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2ba6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2ba6-111">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="e2ba6-111">agreementFileId</span></span>|<span data-ttu-id="e2ba6-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2ba6-112">String</span></span>|<span data-ttu-id="e2ba6-113">Die ID der Vereinbarung-Datei, die vom Benutzer angenommen.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-113">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="e2ba6-114">agreementId</span><span class="sxs-lookup"><span data-stu-id="e2ba6-114">agreementId</span></span>|<span data-ttu-id="e2ba6-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2ba6-115">String</span></span>|<span data-ttu-id="e2ba6-116">ID des zu.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-116">ID of the agreement.</span></span>|
|<span data-ttu-id="e2ba6-117">id</span><span class="sxs-lookup"><span data-stu-id="e2ba6-117">id</span></span>|<span data-ttu-id="e2ba6-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2ba6-118">String</span></span>| <span data-ttu-id="e2ba6-119">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-119">Read-only.</span></span>|
|<span data-ttu-id="e2ba6-120">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2ba6-120">recordedDateTime</span></span>|<span data-ttu-id="e2ba6-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2ba6-121">DateTimeOffset</span></span>|<span data-ttu-id="e2ba6-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e2ba6-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e2ba6-124">state</span><span class="sxs-lookup"><span data-stu-id="e2ba6-124">state</span></span>|<span data-ttu-id="e2ba6-125">string</span><span class="sxs-lookup"><span data-stu-id="e2ba6-125">string</span></span>| <span data-ttu-id="e2ba6-126">Mögliche Werte sind: `accepted` und `declined`.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-126">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="e2ba6-127">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e2ba6-127">userDisplayName</span></span>|<span data-ttu-id="e2ba6-128">String</span><span class="sxs-lookup"><span data-stu-id="e2ba6-128">String</span></span>|<span data-ttu-id="e2ba6-129">Der Anzeigename des Benutzers, wenn die Annahme aufgezeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-129">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e2ba6-130">userEmail</span><span class="sxs-lookup"><span data-stu-id="e2ba6-130">userEmail</span></span>|<span data-ttu-id="e2ba6-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2ba6-131">String</span></span>|<span data-ttu-id="e2ba6-132">E-Mail des Benutzers, wenn die Annahme aufgezeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-132">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e2ba6-133">userId</span><span class="sxs-lookup"><span data-stu-id="e2ba6-133">userId</span></span>|<span data-ttu-id="e2ba6-134">String</span><span class="sxs-lookup"><span data-stu-id="e2ba6-134">String</span></span>|<span data-ttu-id="e2ba6-135">ID des Benutzers, der den Lizenzvertrag akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-135">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="e2ba6-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e2ba6-136">userPrincipalName</span></span>|<span data-ttu-id="e2ba6-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2ba6-137">String</span></span>|<span data-ttu-id="e2ba6-138">UPN des Benutzers, wenn die Annahme aufgezeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-138">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2ba6-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e2ba6-139">Relationships</span></span>
<span data-ttu-id="e2ba6-140">Keine</span><span class="sxs-lookup"><span data-stu-id="e2ba6-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e2ba6-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2ba6-141">JSON representation</span></span>

<span data-ttu-id="e2ba6-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2ba6-142">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
