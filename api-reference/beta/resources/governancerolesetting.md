---
title: Ressourcentyp governanceRoleSetting
description: " Regel, und So weiter."
localization_priority: Normal
ms.openlocfilehash: d63685ae1a4383ce7ab245dda0fd7d1207c57f88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805887"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="b660e-103">Ressourcentyp governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="b660e-103">governanceRoleSetting resource type</span></span>

> <span data-ttu-id="b660e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b660e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b660e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b660e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b660e-106">Stellt eine Reihe von Konfigurationen auf jede Rollendefinition, die ausgewertet werden, wenn rollenzuweisungen erstellt oder geändert werden muss.</span><span class="sxs-lookup"><span data-stu-id="b660e-106">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="b660e-107">Beispielsweise können Einstellungen für Serverrollen Regel "Dauer maximale Zuordnung", "Mehrstufiger Authentifizierung das erforderlich für die Aktivierung" Regel usw. enthalten.</span><span class="sxs-lookup"><span data-stu-id="b660e-107">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="b660e-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="b660e-108">Methods</span></span>

| <span data-ttu-id="b660e-109">Methode</span><span class="sxs-lookup"><span data-stu-id="b660e-109">Method</span></span>          | <span data-ttu-id="b660e-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b660e-110">Return Type</span></span> |<span data-ttu-id="b660e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b660e-111">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="b660e-112">List</span><span class="sxs-lookup"><span data-stu-id="b660e-112">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="b660e-113">[GovernanceRoleSetting](../resources/governancerolesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b660e-113">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="b660e-114">Eine Auflistung von Einstellungen für Serverrollen auf eine Ressource aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="b660e-114">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="b660e-115">Get</span><span class="sxs-lookup"><span data-stu-id="b660e-115">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="b660e-116">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="b660e-116">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="b660e-117">Lesen Sie Eigenschaften und Beziehungen einer Rolle-Einstellung.</span><span class="sxs-lookup"><span data-stu-id="b660e-117">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="b660e-118">Update</span><span class="sxs-lookup"><span data-stu-id="b660e-118">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="b660e-119">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="b660e-119">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="b660e-120">Aktualisieren einer Einstellungsobjekt für die Rolle.</span><span class="sxs-lookup"><span data-stu-id="b660e-120">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b660e-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b660e-121">Properties</span></span>
|<span data-ttu-id="b660e-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b660e-122">Property</span></span>               |<span data-ttu-id="b660e-123">Typ</span><span class="sxs-lookup"><span data-stu-id="b660e-123">Type</span></span>                                      |<span data-ttu-id="b660e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b660e-124">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="b660e-125">id</span><span class="sxs-lookup"><span data-stu-id="b660e-125">id</span></span>                   |<span data-ttu-id="b660e-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b660e-126">String</span></span>                                  |<span data-ttu-id="b660e-127">Die Id des der RoleSetting.</span><span class="sxs-lookup"><span data-stu-id="b660e-127">The id of the roleSetting.</span></span>|
|<span data-ttu-id="b660e-128">resourceId</span><span class="sxs-lookup"><span data-stu-id="b660e-128">resourceId</span></span>           |<span data-ttu-id="b660e-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b660e-129">String</span></span>                                  |<span data-ttu-id="b660e-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b660e-130">Required.</span></span> <span data-ttu-id="b660e-131">Die Id der Ressource, der die Einstellung der Rolle zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="b660e-131">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="b660e-132">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b660e-132">roleDefinitionId</span></span>     |<span data-ttu-id="b660e-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b660e-133">String</span></span>                                  |<span data-ttu-id="b660e-134">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b660e-134">Required.</span></span> <span data-ttu-id="b660e-135">Die Id der Rollendefinition, der die Einstellung der Rolle zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="b660e-135">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="b660e-136">isDefault</span><span class="sxs-lookup"><span data-stu-id="b660e-136">isDefault</span></span>            |<span data-ttu-id="b660e-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b660e-137">Boolean</span></span>                                 |<span data-ttu-id="b660e-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b660e-138">Read-only.</span></span> <span data-ttu-id="b660e-139">Gibt an, ob die RoleSetting eine standardmäßige RoleSetting ist</span><span class="sxs-lookup"><span data-stu-id="b660e-139">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="b660e-140">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b660e-140">lastUpdatedDateTime</span></span>  |<span data-ttu-id="b660e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b660e-141">DateTimeOffset</span></span>                          |<span data-ttu-id="b660e-142">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b660e-142">Read-only.</span></span> <span data-ttu-id="b660e-143">Der Zeitpunkt, wann die Rolle Einstellung zuletzt aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="b660e-143">The time when the role setting was last updated.</span></span> <span data-ttu-id="b660e-144">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="b660e-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b660e-145">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b660e-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b660e-146">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="b660e-146">lastUpdatedBy</span></span>        |<span data-ttu-id="b660e-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b660e-147">String</span></span>                                  |<span data-ttu-id="b660e-148">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b660e-148">Read-only.</span></span> <span data-ttu-id="b660e-149">Der Anzeigename des Administrators, der die RoleSetting zuletzt aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="b660e-149">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="b660e-150">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="b660e-150">adminEligibleSettings</span></span>|<span data-ttu-id="b660e-151">[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b660e-151">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b660e-152">Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="b660e-152">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="b660e-153">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="b660e-153">adminMemberSettings</span></span>  |<span data-ttu-id="b660e-154">[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b660e-154">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b660e-155">Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine direkte rollenzuweisung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="b660e-155">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="b660e-156">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="b660e-156">userEligibleSettings</span></span> |<span data-ttu-id="b660e-157">[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b660e-157">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b660e-158">Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="b660e-158">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="b660e-159">Die Einstellung wird derzeit nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b660e-159">The setting is not supported for now.</span></span>|
|<span data-ttu-id="b660e-160">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="b660e-160">userMemberSettings</span></span>   |<span data-ttu-id="b660e-161">[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b660e-161">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b660e-162">Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, seine rollenzuweisung aktivieren.</span><span class="sxs-lookup"><span data-stu-id="b660e-162">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b660e-163">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b660e-163">Relationships</span></span>
| <span data-ttu-id="b660e-164">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b660e-164">Relationship</span></span> | <span data-ttu-id="b660e-165">Typ</span><span class="sxs-lookup"><span data-stu-id="b660e-165">Type</span></span>   |<span data-ttu-id="b660e-166">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b660e-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b660e-167">resource</span><span class="sxs-lookup"><span data-stu-id="b660e-167">resource</span></span>|[<span data-ttu-id="b660e-168">governanceResource</span><span class="sxs-lookup"><span data-stu-id="b660e-168">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="b660e-169">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b660e-169">Read-only.</span></span> <span data-ttu-id="b660e-170">Die zugeordneten Ressource für diese Rolle-Einstellung.</span><span class="sxs-lookup"><span data-stu-id="b660e-170">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="b660e-171">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b660e-171">roleDefinition</span></span>|[<span data-ttu-id="b660e-172">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b660e-172">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="b660e-173">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b660e-173">Read-only.</span></span> <span data-ttu-id="b660e-174">Die Rollendefinition, die erzwungen wird mit dieser Einstellung Rolle.</span><span class="sxs-lookup"><span data-stu-id="b660e-174">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b660e-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b660e-175">JSON representation</span></span>

<span data-ttu-id="b660e-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b660e-176">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "adminMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
