---
title: Ressourcentyp agreementAcceptance
description: Den aktuellen Status der ein Benutzer innerhalb eines Unternehmens anpassbare rechtliche Hinweise von Azure Active Directory (AD Azure) basiertes Bereichs darstellt.
ms.openlocfilehash: 23221fe88a65b003c8d26aca99eaf1f03d935722
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058145"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="4b7be-103">Ressourcentyp agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="4b7be-103">agreementAcceptance resource type</span></span>

> <span data-ttu-id="4b7be-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4b7be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b7be-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b7be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b7be-106">Den aktuellen Status der ein Benutzer innerhalb eines Unternehmens anpassbare rechtliche Hinweise von Azure Active Directory (AD Azure) basiertes Bereichs darstellt.</span><span class="sxs-lookup"><span data-stu-id="4b7be-106">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="4b7be-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4b7be-107">Properties</span></span>
| <span data-ttu-id="4b7be-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b7be-108">Property</span></span>     | <span data-ttu-id="4b7be-109">Typ</span><span class="sxs-lookup"><span data-stu-id="4b7be-109">Type</span></span>        | <span data-ttu-id="4b7be-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b7be-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4b7be-111">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="4b7be-111">agreementFileId</span></span>|<span data-ttu-id="4b7be-112">String</span><span class="sxs-lookup"><span data-stu-id="4b7be-112">String</span></span>|<span data-ttu-id="4b7be-113">Die ID der Vereinbarung-Datei, die vom Benutzer angenommen.</span><span class="sxs-lookup"><span data-stu-id="4b7be-113">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="4b7be-114">agreementId</span><span class="sxs-lookup"><span data-stu-id="4b7be-114">agreementId</span></span>|<span data-ttu-id="4b7be-115">String</span><span class="sxs-lookup"><span data-stu-id="4b7be-115">String</span></span>|<span data-ttu-id="4b7be-116">ID des zu.</span><span class="sxs-lookup"><span data-stu-id="4b7be-116">ID of the agreement.</span></span>|
|<span data-ttu-id="4b7be-117">id</span><span class="sxs-lookup"><span data-stu-id="4b7be-117">id</span></span>|<span data-ttu-id="4b7be-118">String</span><span class="sxs-lookup"><span data-stu-id="4b7be-118">String</span></span>| <span data-ttu-id="4b7be-119">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4b7be-119">Read-only.</span></span>|
|<span data-ttu-id="4b7be-120">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b7be-120">recordedDateTime</span></span>|<span data-ttu-id="4b7be-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b7be-121">DateTimeOffset</span></span>|<span data-ttu-id="4b7be-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4b7be-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4b7be-124">state</span><span class="sxs-lookup"><span data-stu-id="4b7be-124">state</span></span>|<span data-ttu-id="4b7be-125">string</span><span class="sxs-lookup"><span data-stu-id="4b7be-125">string</span></span>| <span data-ttu-id="4b7be-126">Mögliche Werte sind: `accepted` und `declined`.</span><span class="sxs-lookup"><span data-stu-id="4b7be-126">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="4b7be-127">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4b7be-127">userDisplayName</span></span>|<span data-ttu-id="4b7be-128">String</span><span class="sxs-lookup"><span data-stu-id="4b7be-128">String</span></span>|<span data-ttu-id="4b7be-129">Der Anzeigename des Benutzers, wenn die Annahme aufgezeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="4b7be-129">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="4b7be-130">userEmail</span><span class="sxs-lookup"><span data-stu-id="4b7be-130">userEmail</span></span>|<span data-ttu-id="4b7be-131">String</span><span class="sxs-lookup"><span data-stu-id="4b7be-131">String</span></span>|<span data-ttu-id="4b7be-132">E-Mail des Benutzers, wenn die Annahme aufgezeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="4b7be-132">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="4b7be-133">userId</span><span class="sxs-lookup"><span data-stu-id="4b7be-133">userId</span></span>|<span data-ttu-id="4b7be-134">String</span><span class="sxs-lookup"><span data-stu-id="4b7be-134">String</span></span>|<span data-ttu-id="4b7be-135">ID des Benutzers, der den Lizenzvertrag akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="4b7be-135">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="4b7be-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4b7be-136">userPrincipalName</span></span>|<span data-ttu-id="4b7be-137">String</span><span class="sxs-lookup"><span data-stu-id="4b7be-137">String</span></span>|<span data-ttu-id="4b7be-138">UPN des Benutzers, wenn die Annahme aufgezeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="4b7be-138">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b7be-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4b7be-139">Relationships</span></span>
<span data-ttu-id="4b7be-140">Keine</span><span class="sxs-lookup"><span data-stu-id="4b7be-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4b7be-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4b7be-141">JSON representation</span></span>

<span data-ttu-id="4b7be-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4b7be-142">The following is a JSON representation of the resource.</span></span>

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
