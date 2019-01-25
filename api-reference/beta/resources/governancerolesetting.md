---
title: Ressourcentyp governanceRoleSetting
description: " Regel, und So weiter."
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508167"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="77ce4-103">Ressourcentyp governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="77ce4-103">governanceRoleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77ce4-104">Stellt eine Reihe von Konfigurationen auf jede Rollendefinition, die ausgewertet werden, wenn rollenzuweisungen erstellt oder geändert werden muss.</span><span class="sxs-lookup"><span data-stu-id="77ce4-104">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="77ce4-105">Beispielsweise können Einstellungen für Serverrollen Regel "Dauer maximale Zuordnung", "Mehrstufiger Authentifizierung das erforderlich für die Aktivierung" Regel usw. enthalten.</span><span class="sxs-lookup"><span data-stu-id="77ce4-105">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="77ce4-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="77ce4-106">Methods</span></span>

| <span data-ttu-id="77ce4-107">Methode</span><span class="sxs-lookup"><span data-stu-id="77ce4-107">Method</span></span>          | <span data-ttu-id="77ce4-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="77ce4-108">Return Type</span></span> |<span data-ttu-id="77ce4-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77ce4-109">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="77ce4-110">List</span><span class="sxs-lookup"><span data-stu-id="77ce4-110">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="77ce4-111">[GovernanceRoleSetting](../resources/governancerolesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="77ce4-111">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="77ce4-112">Eine Auflistung von Einstellungen für Serverrollen auf eine Ressource aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="77ce4-112">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="77ce4-113">Get</span><span class="sxs-lookup"><span data-stu-id="77ce4-113">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="77ce4-114">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="77ce4-114">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="77ce4-115">Lesen Sie Eigenschaften und Beziehungen einer Rolle-Einstellung.</span><span class="sxs-lookup"><span data-stu-id="77ce4-115">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="77ce4-116">Update</span><span class="sxs-lookup"><span data-stu-id="77ce4-116">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="77ce4-117">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="77ce4-117">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="77ce4-118">Aktualisieren einer Einstellungsobjekt für die Rolle.</span><span class="sxs-lookup"><span data-stu-id="77ce4-118">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="77ce4-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77ce4-119">Properties</span></span>
|<span data-ttu-id="77ce4-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77ce4-120">Property</span></span>               |<span data-ttu-id="77ce4-121">Typ</span><span class="sxs-lookup"><span data-stu-id="77ce4-121">Type</span></span>                                      |<span data-ttu-id="77ce4-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77ce4-122">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="77ce4-123">id</span><span class="sxs-lookup"><span data-stu-id="77ce4-123">id</span></span>                   |<span data-ttu-id="77ce4-124">String</span><span class="sxs-lookup"><span data-stu-id="77ce4-124">String</span></span>                                  |<span data-ttu-id="77ce4-125">Die Id des der RoleSetting.</span><span class="sxs-lookup"><span data-stu-id="77ce4-125">The id of the roleSetting.</span></span>|
|<span data-ttu-id="77ce4-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="77ce4-126">resourceId</span></span>           |<span data-ttu-id="77ce4-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77ce4-127">String</span></span>                                  |<span data-ttu-id="77ce4-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77ce4-128">Required.</span></span> <span data-ttu-id="77ce4-129">Die Id der Ressource, der die Einstellung der Rolle zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="77ce4-129">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="77ce4-130">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="77ce4-130">roleDefinitionId</span></span>     |<span data-ttu-id="77ce4-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77ce4-131">String</span></span>                                  |<span data-ttu-id="77ce4-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77ce4-132">Required.</span></span> <span data-ttu-id="77ce4-133">Die Id der Rollendefinition, der die Einstellung der Rolle zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="77ce4-133">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="77ce4-134">isDefault</span><span class="sxs-lookup"><span data-stu-id="77ce4-134">isDefault</span></span>            |<span data-ttu-id="77ce4-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77ce4-135">Boolean</span></span>                                 |<span data-ttu-id="77ce4-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="77ce4-136">Read-only.</span></span> <span data-ttu-id="77ce4-137">Gibt an, ob die RoleSetting eine standardmäßige RoleSetting ist</span><span class="sxs-lookup"><span data-stu-id="77ce4-137">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="77ce4-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="77ce4-138">lastUpdatedDateTime</span></span>  |<span data-ttu-id="77ce4-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77ce4-139">DateTimeOffset</span></span>                          |<span data-ttu-id="77ce4-140">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="77ce4-140">Read-only.</span></span> <span data-ttu-id="77ce4-141">Der Zeitpunkt, wann die Rolle Einstellung zuletzt aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="77ce4-141">The time when the role setting was last updated.</span></span> <span data-ttu-id="77ce4-142">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="77ce4-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="77ce4-143">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="77ce4-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="77ce4-144">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="77ce4-144">lastUpdatedBy</span></span>        |<span data-ttu-id="77ce4-145">String</span><span class="sxs-lookup"><span data-stu-id="77ce4-145">String</span></span>                                  |<span data-ttu-id="77ce4-146">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="77ce4-146">Read-only.</span></span> <span data-ttu-id="77ce4-147">Der Anzeigename des Administrators, der die RoleSetting zuletzt aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="77ce4-147">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="77ce4-148">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="77ce4-148">adminEligibleSettings</span></span>|<span data-ttu-id="77ce4-149">[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="77ce4-149">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="77ce4-150">Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="77ce4-150">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="77ce4-151">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="77ce4-151">adminMemberSettings</span></span>  |<span data-ttu-id="77ce4-152">[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="77ce4-152">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="77ce4-153">Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine direkte rollenzuweisung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="77ce4-153">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="77ce4-154">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="77ce4-154">userEligibleSettings</span></span> |<span data-ttu-id="77ce4-155">[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="77ce4-155">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="77ce4-156">Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="77ce4-156">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="77ce4-157">Die Einstellung wird derzeit nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77ce4-157">The setting is not supported for now.</span></span>|
|<span data-ttu-id="77ce4-158">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="77ce4-158">userMemberSettings</span></span>   |<span data-ttu-id="77ce4-159">[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="77ce4-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="77ce4-160">Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, seine rollenzuweisung aktivieren.</span><span class="sxs-lookup"><span data-stu-id="77ce4-160">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77ce4-161">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="77ce4-161">Relationships</span></span>
| <span data-ttu-id="77ce4-162">Beziehung</span><span class="sxs-lookup"><span data-stu-id="77ce4-162">Relationship</span></span> | <span data-ttu-id="77ce4-163">Typ</span><span class="sxs-lookup"><span data-stu-id="77ce4-163">Type</span></span>   |<span data-ttu-id="77ce4-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77ce4-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77ce4-165">resource</span><span class="sxs-lookup"><span data-stu-id="77ce4-165">resource</span></span>|[<span data-ttu-id="77ce4-166">governanceResource</span><span class="sxs-lookup"><span data-stu-id="77ce4-166">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="77ce4-167">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="77ce4-167">Read-only.</span></span> <span data-ttu-id="77ce4-168">Die zugeordneten Ressource für diese Rolle-Einstellung.</span><span class="sxs-lookup"><span data-stu-id="77ce4-168">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="77ce4-169">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="77ce4-169">roleDefinition</span></span>|[<span data-ttu-id="77ce4-170">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="77ce4-170">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="77ce4-171">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="77ce4-171">Read-only.</span></span> <span data-ttu-id="77ce4-172">Die Rollendefinition, die erzwungen wird mit dieser Einstellung Rolle.</span><span class="sxs-lookup"><span data-stu-id="77ce4-172">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="77ce4-173">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77ce4-173">JSON representation</span></span>

<span data-ttu-id="77ce4-174">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77ce4-174">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerolesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
