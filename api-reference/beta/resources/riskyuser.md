---
title: riskyUsers-Ressourcentyp
description: Stellt Azure AD-Benutzer dar, die gefährdet sind. Azure AD bewertet das Benutzer Risiko kontinuierlich anhand verschiedener Signale und des maschinellen Lernens. Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3265ea40903ca2c5c10272f5df280bd3715af366
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003720"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="14918-105">riskyUsers-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="14918-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14918-106">Stellt Azure AD-Benutzer dar, die gefährdet sind.</span><span class="sxs-lookup"><span data-stu-id="14918-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="14918-107">Azure AD bewertet das Benutzer Risiko kontinuierlich anhand verschiedener Signale und des maschinellen Lernens.</span><span class="sxs-lookup"><span data-stu-id="14918-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="14918-108">Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="14918-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="14918-109">Weitere Informationen zu Risikoereignissen finden Sie unter [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="14918-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="14918-110">**Hinweis:** Die Verwendung der riskyUsers-API erfordert eine Azure AD Premium P2-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="14918-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="14918-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="14918-111">Methods</span></span>

| <span data-ttu-id="14918-112">Methode</span><span class="sxs-lookup"><span data-stu-id="14918-112">Method</span></span>   | <span data-ttu-id="14918-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="14918-113">Return Type</span></span>|<span data-ttu-id="14918-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14918-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="14918-115">RiskyUsers aufListen</span><span class="sxs-lookup"><span data-stu-id="14918-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="14918-116">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="14918-116">riskyUsers</span></span>](riskyUser.md) |<span data-ttu-id="14918-117">AufListen von riskanten Benutzern und deren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="14918-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="14918-118">RiskyUsers abrufen</span><span class="sxs-lookup"><span data-stu-id="14918-118">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="14918-119">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="14918-119">riskyUsers</span></span>](riskyUser.md)|<span data-ttu-id="14918-120">Abrufen eines bestimmten riskanten Benutzers und seiner Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="14918-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="14918-121">Bestätigen der riskyUsers kompromittiert</span><span class="sxs-lookup"><span data-stu-id="14918-121">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="14918-122">Bestätigen Sie einen riskanten Benutzer als kompromittiert.</span><span class="sxs-lookup"><span data-stu-id="14918-122">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="14918-123">RiskyUsers schließen</span><span class="sxs-lookup"><span data-stu-id="14918-123">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="14918-124">Schließen Sie das Risiko eines riskanten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="14918-124">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="14918-125">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="14918-125">Properties</span></span>

| <span data-ttu-id="14918-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14918-126">Property</span></span>   | <span data-ttu-id="14918-127">Typ</span><span class="sxs-lookup"><span data-stu-id="14918-127">Type</span></span>|<span data-ttu-id="14918-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14918-128">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="14918-129">Eindeutige ID des gefährdeten Benutzers</span><span class="sxs-lookup"><span data-stu-id="14918-129">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="14918-130">Gibt an, ob der Benutzer gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="14918-130">Indicates whether the user is deleted.</span></span> <span data-ttu-id="14918-131">Mögliche Werte sind: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="14918-131">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="14918-132">Gibt an, ob der Benutzer ein Gastbenutzer ist.</span><span class="sxs-lookup"><span data-stu-id="14918-132">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="14918-133">Mögliche Werte sind: `true` und `false`.</span><span class="sxs-lookup"><span data-stu-id="14918-133">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="14918-134">True, wenn die Identität des Benutzers außerhalb des Mandanten liegt.</span><span class="sxs-lookup"><span data-stu-id="14918-134">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="14918-135">Dieser Benutzer kann ein B2B-oder ein B2C-Benutzer mit Identität in Azure AD, MSA oder Drittanbieter-Identitätsanbieter sein.</span><span class="sxs-lookup"><span data-stu-id="14918-135">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="14918-136">False, wenn die Identität des Benutzers in Betracht gezogen wird</span><span class="sxs-lookup"><span data-stu-id="14918-136">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="14918-137">Gibt an, wehther der riskante Status eines Benutzers vom Back-End verarbeitet wird.</span><span class="sxs-lookup"><span data-stu-id="14918-137">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`risk`|[<span data-ttu-id="14918-138">Risiko</span><span class="sxs-lookup"><span data-stu-id="14918-138">risk</span></span>](risk.md)|<span data-ttu-id="14918-139">Riskanter Benutzerstatus</span><span class="sxs-lookup"><span data-stu-id="14918-139">Risky user state</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="14918-140">Datum und Uhrzeit der letzten Aktualisierung des Risiko Benutzer</span><span class="sxs-lookup"><span data-stu-id="14918-140">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="14918-141">Riskanter Benutzeranzeigename</span><span class="sxs-lookup"><span data-stu-id="14918-141">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="14918-142">Riskanter Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="14918-142">Risky user principal name</span></span>|


## <a name="json-representation"></a><span data-ttu-id="14918-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="14918-143">JSON representation</span></span>

<span data-ttu-id="14918-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="14918-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
 "id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isProcessing": "boolean",
"isDeleted": "boolean",
"risk": {"@odata.type": "microsoft.graph.risk"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
