---
title: deviceAndAppManagementRoleDefinition-Ressourcentyp
description: 'Die Rollendefinitionsressource. Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune. In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert. Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen. Integrierte Rollen können nicht geändert werden. Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden. Erstellen Sie benutzerdefinierte Rollen, wenn Sie eine Rolle definieren möchten, in der beliebige der verfügbaren Ressourcen und Rollenberechtigungen kombiniert werden können.'
ms.openlocfilehash: 90c701afc33a16cfb2747c40d53d47e74c3cedde
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061412"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="2061f-109">deviceAndAppManagementRoleDefinition-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2061f-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="2061f-110">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2061f-110">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2061f-111">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2061f-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2061f-112">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2061f-112">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2061f-113">Die Rollendefinitionsressource.</span><span class="sxs-lookup"><span data-stu-id="2061f-113">The Role Definition resource.</span></span> <span data-ttu-id="2061f-114">Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune.</span><span class="sxs-lookup"><span data-stu-id="2061f-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="2061f-115">In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert.</span><span class="sxs-lookup"><span data-stu-id="2061f-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="2061f-116">Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="2061f-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="2061f-117">Integrierte Rollen können nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="2061f-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="2061f-118">Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden.</span><span class="sxs-lookup"><span data-stu-id="2061f-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="2061f-119">Erstellen Sie benutzerdefinierte Rollen, wenn Sie eine Rolle definieren möchten, in der beliebige der verfügbaren Ressourcen und Rollenberechtigungen kombiniert werden können.</span><span class="sxs-lookup"><span data-stu-id="2061f-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

<span data-ttu-id="2061f-120">Erbt von [RoleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2061f-121">Methoden</span><span class="sxs-lookup"><span data-stu-id="2061f-121">Methods</span></span>
|<span data-ttu-id="2061f-122">Methode</span><span class="sxs-lookup"><span data-stu-id="2061f-122">Method</span></span>|<span data-ttu-id="2061f-123">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2061f-123">Return Type</span></span>|<span data-ttu-id="2061f-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2061f-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2061f-125">deviceAndAppManagementRoleDefinitions auflisten</span><span class="sxs-lookup"><span data-stu-id="2061f-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="2061f-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2061f-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="2061f-127">Auflisten von Eigenschaften und Beziehungen der [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="2061f-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="2061f-128">deviceAndAppManagementRoleDefinition abrufen</span><span class="sxs-lookup"><span data-stu-id="2061f-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="2061f-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2061f-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="2061f-130">Lesen von Eigenschaften und Beziehungen des [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2061f-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="2061f-131">deviceAndAppManagementRoleDefinition erstellen</span><span class="sxs-lookup"><span data-stu-id="2061f-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="2061f-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2061f-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="2061f-133">Erstellen eines neuen [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2061f-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="2061f-134">deviceAndAppManagementRoleDefinition löschen</span><span class="sxs-lookup"><span data-stu-id="2061f-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="2061f-135">Keine</span><span class="sxs-lookup"><span data-stu-id="2061f-135">None</span></span>|<span data-ttu-id="2061f-136">Löscht ein [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="2061f-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="2061f-137">deviceAndAppManagementRoleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2061f-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="2061f-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2061f-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="2061f-139">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2061f-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2061f-140">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2061f-140">Properties</span></span>
|<span data-ttu-id="2061f-141">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2061f-141">Property</span></span>|<span data-ttu-id="2061f-142">Typ</span><span class="sxs-lookup"><span data-stu-id="2061f-142">Type</span></span>|<span data-ttu-id="2061f-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2061f-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2061f-144">id</span><span class="sxs-lookup"><span data-stu-id="2061f-144">id</span></span>|<span data-ttu-id="2061f-145">String</span><span class="sxs-lookup"><span data-stu-id="2061f-145">String</span></span>|<span data-ttu-id="2061f-146">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2061f-146">Key of the entity.</span></span> <span data-ttu-id="2061f-147">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="2061f-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="2061f-148">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2061f-149">displayName</span><span class="sxs-lookup"><span data-stu-id="2061f-149">displayName</span></span>|<span data-ttu-id="2061f-150">String</span><span class="sxs-lookup"><span data-stu-id="2061f-150">String</span></span>|<span data-ttu-id="2061f-151">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="2061f-151">Display Name of the Role definition.</span></span> <span data-ttu-id="2061f-152">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2061f-153">description</span><span class="sxs-lookup"><span data-stu-id="2061f-153">description</span></span>|<span data-ttu-id="2061f-154">String</span><span class="sxs-lookup"><span data-stu-id="2061f-154">String</span></span>|<span data-ttu-id="2061f-155">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="2061f-155">Description of the Role definition.</span></span> <span data-ttu-id="2061f-156">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2061f-157">permissions</span><span class="sxs-lookup"><span data-stu-id="2061f-157">permissions</span></span>|<span data-ttu-id="2061f-158">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="2061f-159">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="2061f-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="2061f-160">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="2061f-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="2061f-161">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2061f-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="2061f-162">rolePermissions</span></span>|<span data-ttu-id="2061f-163">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="2061f-164">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="2061f-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="2061f-165">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="2061f-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="2061f-166">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2061f-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2061f-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="2061f-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2061f-168">Boolean</span></span>|<span data-ttu-id="2061f-169">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="2061f-169">Type of Role.</span></span> <span data-ttu-id="2061f-170">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="2061f-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="2061f-171">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2061f-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="2061f-172">isBuiltIn</span></span>|<span data-ttu-id="2061f-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2061f-173">Boolean</span></span>|<span data-ttu-id="2061f-174">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="2061f-174">Type of Role.</span></span> <span data-ttu-id="2061f-175">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="2061f-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="2061f-176">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2061f-177">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2061f-177">Relationships</span></span>
|<span data-ttu-id="2061f-178">Beziehung</span><span class="sxs-lookup"><span data-stu-id="2061f-178">Relationship</span></span>|<span data-ttu-id="2061f-179">Typ</span><span class="sxs-lookup"><span data-stu-id="2061f-179">Type</span></span>|<span data-ttu-id="2061f-180">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2061f-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2061f-181">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="2061f-181">roleAssignments</span></span>|<span data-ttu-id="2061f-182">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-182">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="2061f-183">Liste von Rollenzuweisungen für diese Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="2061f-183">List of Role assignments for this role definition.</span></span> <span data-ttu-id="2061f-184">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2061f-184">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2061f-185">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2061f-185">JSON Representation</span></span>
<span data-ttu-id="2061f-186">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2061f-186">Here is a JSON representation of the resource.</span></span>
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
  "isBuiltIn": true
}
```





