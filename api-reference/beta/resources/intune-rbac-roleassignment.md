---
title: roleAssignment-Ressourcentyp
description: Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.
author: tfitzmac
ms.openlocfilehash: 5c4b09151a7957f52dbaa525f696b89479a898ef
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302100"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="e48d2-106">roleAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e48d2-106">roleAssignment resource type</span></span>

> <span data-ttu-id="e48d2-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e48d2-107">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e48d2-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e48d2-108">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e48d2-109">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e48d2-109">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e48d2-110">Die Rollenzuweisungsressource.</span><span class="sxs-lookup"><span data-stu-id="e48d2-110">The Role Assignment resource.</span></span> <span data-ttu-id="e48d2-111">Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen.</span><span class="sxs-lookup"><span data-stu-id="e48d2-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="e48d2-112">Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben.</span><span class="sxs-lookup"><span data-stu-id="e48d2-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="e48d2-113">Dies gilt für benutzerdefinierte und integrierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="e48d2-113">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="e48d2-114">Methoden</span><span class="sxs-lookup"><span data-stu-id="e48d2-114">Methods</span></span>
|<span data-ttu-id="e48d2-115">Methode</span><span class="sxs-lookup"><span data-stu-id="e48d2-115">Method</span></span>|<span data-ttu-id="e48d2-116">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e48d2-116">Return Type</span></span>|<span data-ttu-id="e48d2-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e48d2-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e48d2-118">RoleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="e48d2-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="e48d2-119">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e48d2-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="e48d2-120">Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="e48d2-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="e48d2-121">RoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="e48d2-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="e48d2-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="e48d2-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="e48d2-123">Lesen von Eigenschaften und Beziehungen des [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e48d2-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="e48d2-124">RoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="e48d2-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="e48d2-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="e48d2-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="e48d2-126">Erstellen eines neuen [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e48d2-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="e48d2-127">RoleAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="e48d2-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="e48d2-128">Keine</span><span class="sxs-lookup"><span data-stu-id="e48d2-128">None</span></span>|<span data-ttu-id="e48d2-129">Löscht ein [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="e48d2-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="e48d2-130">RoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e48d2-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="e48d2-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="e48d2-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="e48d2-132">Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e48d2-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e48d2-133">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e48d2-133">Properties</span></span>
|<span data-ttu-id="e48d2-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e48d2-134">Property</span></span>|<span data-ttu-id="e48d2-135">Typ</span><span class="sxs-lookup"><span data-stu-id="e48d2-135">Type</span></span>|<span data-ttu-id="e48d2-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e48d2-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e48d2-137">id</span><span class="sxs-lookup"><span data-stu-id="e48d2-137">id</span></span>|<span data-ttu-id="e48d2-138">String</span><span class="sxs-lookup"><span data-stu-id="e48d2-138">String</span></span>|<span data-ttu-id="e48d2-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e48d2-139">Key of the entity.</span></span> <span data-ttu-id="e48d2-140">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="e48d2-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="e48d2-141">displayName</span><span class="sxs-lookup"><span data-stu-id="e48d2-141">displayName</span></span>|<span data-ttu-id="e48d2-142">String</span><span class="sxs-lookup"><span data-stu-id="e48d2-142">String</span></span>|<span data-ttu-id="e48d2-143">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="e48d2-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="e48d2-144">description</span><span class="sxs-lookup"><span data-stu-id="e48d2-144">description</span></span>|<span data-ttu-id="e48d2-145">String</span><span class="sxs-lookup"><span data-stu-id="e48d2-145">String</span></span>|<span data-ttu-id="e48d2-146">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="e48d2-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="e48d2-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="e48d2-147">scopeMembers</span></span>|<span data-ttu-id="e48d2-148">String collection</span><span class="sxs-lookup"><span data-stu-id="e48d2-148">String collection</span></span>|<span data-ttu-id="e48d2-149">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="e48d2-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="e48d2-150">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e48d2-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="e48d2-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="e48d2-151">scopeType</span></span>|[<span data-ttu-id="e48d2-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="e48d2-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="e48d2-153">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="e48d2-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="e48d2-154">Standardtyp 'ResourceScope' ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="e48d2-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="e48d2-155">Für 'AllDevices', 'AllLicensedUsers' und 'AllDevicesAndLicensedUsers' sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="e48d2-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="e48d2-156">Mögliche Werte: sind `resourceScope`, `allDevices`, `allLicensedUsers` und `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="e48d2-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="e48d2-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="e48d2-157">resourceScopes</span></span>|<span data-ttu-id="e48d2-158">String collection</span><span class="sxs-lookup"><span data-stu-id="e48d2-158">String collection</span></span>|<span data-ttu-id="e48d2-159">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="e48d2-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="e48d2-160">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e48d2-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e48d2-161">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e48d2-161">Relationships</span></span>
|<span data-ttu-id="e48d2-162">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e48d2-162">Relationship</span></span>|<span data-ttu-id="e48d2-163">Typ</span><span class="sxs-lookup"><span data-stu-id="e48d2-163">Type</span></span>|<span data-ttu-id="e48d2-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e48d2-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e48d2-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e48d2-165">roleDefinition</span></span>|[<span data-ttu-id="e48d2-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e48d2-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="e48d2-167">Die Rollendefinition, in der diese Zuweisung enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="e48d2-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e48d2-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e48d2-168">JSON Representation</span></span>
<span data-ttu-id="e48d2-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e48d2-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ]
}
```





