---
title: deviceAndAppManagementRoleDefinition-Ressourcentyp
description: 'Die Rollendefinitionsressource. Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune. In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert. Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen. Integrierte Rollen können nicht geändert werden. Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden. Erstellen Sie benutzerdefinierte Rollen, wenn Sie eine Rolle definieren möchten, in der beliebige der verfügbaren Ressourcen und Rollenberechtigungen kombiniert werden können.'
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cc3bd898799ef2c2da6fca5a0043fc86ee5bd8f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411981"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="81dcb-109">deviceAndAppManagementRoleDefinition-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="81dcb-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="81dcb-110">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="81dcb-110">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="81dcb-111">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81dcb-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81dcb-112">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="81dcb-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81dcb-113">Die Rollendefinitionsressource.</span><span class="sxs-lookup"><span data-stu-id="81dcb-113">The Role Definition resource.</span></span> <span data-ttu-id="81dcb-114">Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune.</span><span class="sxs-lookup"><span data-stu-id="81dcb-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="81dcb-115">In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert.</span><span class="sxs-lookup"><span data-stu-id="81dcb-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="81dcb-116">Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="81dcb-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="81dcb-117">Integrierte Rollen können nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="81dcb-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="81dcb-118">Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden.</span><span class="sxs-lookup"><span data-stu-id="81dcb-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="81dcb-119">Erstellen Sie benutzerdefinierte Rollen, wenn Sie eine Rolle definieren möchten, in der beliebige der verfügbaren Ressourcen und Rollenberechtigungen kombiniert werden können.</span><span class="sxs-lookup"><span data-stu-id="81dcb-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="81dcb-120">Erbt von [RoleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="81dcb-121">Methoden</span><span class="sxs-lookup"><span data-stu-id="81dcb-121">Methods</span></span>
|<span data-ttu-id="81dcb-122">Methode</span><span class="sxs-lookup"><span data-stu-id="81dcb-122">Method</span></span>|<span data-ttu-id="81dcb-123">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="81dcb-123">Return Type</span></span>|<span data-ttu-id="81dcb-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81dcb-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81dcb-125">deviceAndAppManagementRoleDefinitions auflisten</span><span class="sxs-lookup"><span data-stu-id="81dcb-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="81dcb-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="81dcb-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="81dcb-127">Auflisten von Eigenschaften und Beziehungen der [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="81dcb-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="81dcb-128">deviceAndAppManagementRoleDefinition abrufen</span><span class="sxs-lookup"><span data-stu-id="81dcb-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="81dcb-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="81dcb-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="81dcb-130">Lesen von Eigenschaften und Beziehungen des [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="81dcb-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="81dcb-131">deviceAndAppManagementRoleDefinition erstellen</span><span class="sxs-lookup"><span data-stu-id="81dcb-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="81dcb-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="81dcb-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="81dcb-133">Erstellen eines neuen [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="81dcb-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="81dcb-134">deviceAndAppManagementRoleDefinition löschen</span><span class="sxs-lookup"><span data-stu-id="81dcb-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="81dcb-135">Keine</span><span class="sxs-lookup"><span data-stu-id="81dcb-135">None</span></span>|<span data-ttu-id="81dcb-136">Löscht ein [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="81dcb-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="81dcb-137">deviceAndAppManagementRoleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="81dcb-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="81dcb-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="81dcb-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="81dcb-139">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="81dcb-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81dcb-140">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="81dcb-140">Properties</span></span>
|<span data-ttu-id="81dcb-141">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81dcb-141">Property</span></span>|<span data-ttu-id="81dcb-142">Typ</span><span class="sxs-lookup"><span data-stu-id="81dcb-142">Type</span></span>|<span data-ttu-id="81dcb-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81dcb-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81dcb-144">id</span><span class="sxs-lookup"><span data-stu-id="81dcb-144">id</span></span>|<span data-ttu-id="81dcb-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81dcb-145">String</span></span>|<span data-ttu-id="81dcb-146">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="81dcb-146">Key of the entity.</span></span> <span data-ttu-id="81dcb-147">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="81dcb-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="81dcb-148">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="81dcb-149">displayName</span><span class="sxs-lookup"><span data-stu-id="81dcb-149">displayName</span></span>|<span data-ttu-id="81dcb-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81dcb-150">String</span></span>|<span data-ttu-id="81dcb-151">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="81dcb-151">Display Name of the Role definition.</span></span> <span data-ttu-id="81dcb-152">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="81dcb-153">description</span><span class="sxs-lookup"><span data-stu-id="81dcb-153">description</span></span>|<span data-ttu-id="81dcb-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81dcb-154">String</span></span>|<span data-ttu-id="81dcb-155">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="81dcb-155">Description of the Role definition.</span></span> <span data-ttu-id="81dcb-156">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="81dcb-157">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="81dcb-157">permissions</span></span>|<span data-ttu-id="81dcb-158">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="81dcb-159">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="81dcb-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="81dcb-160">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="81dcb-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="81dcb-161">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="81dcb-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="81dcb-162">rolePermissions</span></span>|<span data-ttu-id="81dcb-163">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="81dcb-164">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="81dcb-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="81dcb-165">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="81dcb-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="81dcb-166">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="81dcb-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="81dcb-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="81dcb-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="81dcb-168">Boolean</span></span>|<span data-ttu-id="81dcb-169">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="81dcb-169">Type of Role.</span></span> <span data-ttu-id="81dcb-170">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="81dcb-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="81dcb-171">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="81dcb-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="81dcb-172">isBuiltIn</span></span>|<span data-ttu-id="81dcb-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="81dcb-173">Boolean</span></span>|<span data-ttu-id="81dcb-174">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="81dcb-174">Type of Role.</span></span> <span data-ttu-id="81dcb-175">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="81dcb-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="81dcb-176">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="81dcb-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="81dcb-177">roleScopeTagIds</span></span>|<span data-ttu-id="81dcb-178">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="81dcb-178">String collection</span></span>|<span data-ttu-id="81dcb-179">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="81dcb-179">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="81dcb-180">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-180">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="81dcb-181">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="81dcb-181">Relationships</span></span>
|<span data-ttu-id="81dcb-182">Beziehung</span><span class="sxs-lookup"><span data-stu-id="81dcb-182">Relationship</span></span>|<span data-ttu-id="81dcb-183">Typ</span><span class="sxs-lookup"><span data-stu-id="81dcb-183">Type</span></span>|<span data-ttu-id="81dcb-184">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81dcb-184">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81dcb-185">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="81dcb-185">roleAssignments</span></span>|<span data-ttu-id="81dcb-186">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-186">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="81dcb-187">Liste von Rollenzuweisungen für diese Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="81dcb-187">List of Role assignments for this role definition.</span></span> <span data-ttu-id="81dcb-188">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="81dcb-188">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81dcb-189">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="81dcb-189">JSON Representation</span></span>
<span data-ttu-id="81dcb-190">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="81dcb-190">Here is a JSON representation of the resource.</span></span>
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




