---
title: deviceAndAppManagementRoleDefinition-Ressourcentyp
description: 'Die Rollendefinitionsressource. Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune. In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert. Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen. Integrierte Rollen können nicht geändert werden. Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden. Erstellen Sie benutzerdefinierte Rollen, wenn Sie eine Rolle definieren möchten, in der beliebige der verfügbaren Ressourcen und Rollenberechtigungen kombiniert werden können.'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bee2a27e22a44925dfdc9f36a52e0067fbc72cac
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139893"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="bb6da-109">deviceAndAppManagementRoleDefinition-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bb6da-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="bb6da-110">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bb6da-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb6da-111">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bb6da-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb6da-112">Die Rollendefinitionsressource.</span><span class="sxs-lookup"><span data-stu-id="bb6da-112">The Role Definition resource.</span></span> <span data-ttu-id="bb6da-113">Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune.</span><span class="sxs-lookup"><span data-stu-id="bb6da-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="bb6da-114">In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert.</span><span class="sxs-lookup"><span data-stu-id="bb6da-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="bb6da-115">Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="bb6da-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="bb6da-116">Integrierte Rollen können nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="bb6da-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="bb6da-117">Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden.</span><span class="sxs-lookup"><span data-stu-id="bb6da-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="bb6da-118">Erstellen Sie benutzerdefinierte Rollen, wenn Sie eine Rolle definieren möchten, in der beliebige der verfügbaren Ressourcen und Rollenberechtigungen kombiniert werden können.</span><span class="sxs-lookup"><span data-stu-id="bb6da-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="bb6da-119">Erbt von [RoleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-119">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bb6da-120">Methoden</span><span class="sxs-lookup"><span data-stu-id="bb6da-120">Methods</span></span>
|<span data-ttu-id="bb6da-121">Methode</span><span class="sxs-lookup"><span data-stu-id="bb6da-121">Method</span></span>|<span data-ttu-id="bb6da-122">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bb6da-122">Return Type</span></span>|<span data-ttu-id="bb6da-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb6da-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb6da-124">deviceAndAppManagementRoleDefinitions auflisten</span><span class="sxs-lookup"><span data-stu-id="bb6da-124">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="bb6da-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bb6da-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="bb6da-126">Auflisten von Eigenschaften und Beziehungen der [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="bb6da-126">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="bb6da-127">deviceAndAppManagementRoleDefinition abrufen</span><span class="sxs-lookup"><span data-stu-id="bb6da-127">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="bb6da-128">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bb6da-128">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="bb6da-129">Lesen von Eigenschaften und Beziehungen des [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb6da-129">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="bb6da-130">deviceAndAppManagementRoleDefinition erstellen</span><span class="sxs-lookup"><span data-stu-id="bb6da-130">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="bb6da-131">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bb6da-131">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="bb6da-132">Erstellen eines neuen [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb6da-132">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="bb6da-133">deviceAndAppManagementRoleDefinition löschen</span><span class="sxs-lookup"><span data-stu-id="bb6da-133">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="bb6da-134">Keine</span><span class="sxs-lookup"><span data-stu-id="bb6da-134">None</span></span>|<span data-ttu-id="bb6da-135">Löscht ein [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="bb6da-135">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="bb6da-136">deviceAndAppManagementRoleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bb6da-136">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="bb6da-137">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bb6da-137">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="bb6da-138">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb6da-138">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb6da-139">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bb6da-139">Properties</span></span>
|<span data-ttu-id="bb6da-140">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bb6da-140">Property</span></span>|<span data-ttu-id="bb6da-141">Typ</span><span class="sxs-lookup"><span data-stu-id="bb6da-141">Type</span></span>|<span data-ttu-id="bb6da-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb6da-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb6da-143">id</span><span class="sxs-lookup"><span data-stu-id="bb6da-143">id</span></span>|<span data-ttu-id="bb6da-144">String</span><span class="sxs-lookup"><span data-stu-id="bb6da-144">String</span></span>|<span data-ttu-id="bb6da-145">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bb6da-145">Key of the entity.</span></span> <span data-ttu-id="bb6da-146">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="bb6da-146">This is read-only and automatically generated.</span></span> <span data-ttu-id="bb6da-147">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-147">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="bb6da-148">displayName</span><span class="sxs-lookup"><span data-stu-id="bb6da-148">displayName</span></span>|<span data-ttu-id="bb6da-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb6da-149">String</span></span>|<span data-ttu-id="bb6da-150">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="bb6da-150">Display Name of the Role definition.</span></span> <span data-ttu-id="bb6da-151">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-151">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="bb6da-152">description</span><span class="sxs-lookup"><span data-stu-id="bb6da-152">description</span></span>|<span data-ttu-id="bb6da-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb6da-153">String</span></span>|<span data-ttu-id="bb6da-154">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="bb6da-154">Description of the Role definition.</span></span> <span data-ttu-id="bb6da-155">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="bb6da-156">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bb6da-156">permissions</span></span>|<span data-ttu-id="bb6da-157">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="bb6da-158">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="bb6da-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="bb6da-159">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="bb6da-159">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="bb6da-160">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="bb6da-161">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="bb6da-161">rolePermissions</span></span>|<span data-ttu-id="bb6da-162">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-162">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="bb6da-163">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="bb6da-163">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="bb6da-164">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="bb6da-164">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="bb6da-165">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="bb6da-166">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bb6da-166">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="bb6da-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6da-167">Boolean</span></span>|<span data-ttu-id="bb6da-168">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="bb6da-168">Type of Role.</span></span> <span data-ttu-id="bb6da-169">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="bb6da-169">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="bb6da-170">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-170">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="bb6da-171">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="bb6da-171">isBuiltIn</span></span>|<span data-ttu-id="bb6da-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6da-172">Boolean</span></span>|<span data-ttu-id="bb6da-173">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="bb6da-173">Type of Role.</span></span> <span data-ttu-id="bb6da-174">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="bb6da-174">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="bb6da-175">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-175">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="bb6da-176">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="bb6da-176">roleScopeTagIds</span></span>|<span data-ttu-id="bb6da-177">String collection</span><span class="sxs-lookup"><span data-stu-id="bb6da-177">String collection</span></span>|<span data-ttu-id="bb6da-178">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="bb6da-178">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bb6da-179">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-179">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb6da-180">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bb6da-180">Relationships</span></span>
|<span data-ttu-id="bb6da-181">Beziehung</span><span class="sxs-lookup"><span data-stu-id="bb6da-181">Relationship</span></span>|<span data-ttu-id="bb6da-182">Typ</span><span class="sxs-lookup"><span data-stu-id="bb6da-182">Type</span></span>|<span data-ttu-id="bb6da-183">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb6da-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb6da-184">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="bb6da-184">roleAssignments</span></span>|<span data-ttu-id="bb6da-185">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-185">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="bb6da-186">Liste von Rollenzuweisungen für diese Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="bb6da-186">List of Role assignments for this role definition.</span></span> <span data-ttu-id="bb6da-187">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb6da-187">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb6da-188">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bb6da-188">JSON Representation</span></span>
<span data-ttu-id="bb6da-189">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bb6da-189">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




