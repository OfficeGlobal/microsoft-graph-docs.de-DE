---
title: Ressourcentyp „roleDefinition“
description: 'Die Rollendefinitionsressource. Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune. In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert. Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen. Integrierte Rollen können nicht geändert werden. Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden. Erstellen Sie benutzerdefinierte Rollen, wenn Sie eine Rolle definieren möchten, in der beliebige der verfügbaren Ressourcen und Rollenberechtigungen kombiniert werden können.'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba38f9293ce4a21d031a3c70e8d3bdbe5667f997
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173717"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="e9341-109">Ressourcentyp „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="e9341-109">roleDefinition resource type</span></span>

> <span data-ttu-id="e9341-110">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e9341-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9341-111">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e9341-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9341-112">Die Rollendefinitionsressource.</span><span class="sxs-lookup"><span data-stu-id="e9341-112">The Role Definition resource.</span></span> <span data-ttu-id="e9341-113">Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune.</span><span class="sxs-lookup"><span data-stu-id="e9341-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="e9341-114">In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert.</span><span class="sxs-lookup"><span data-stu-id="e9341-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="e9341-115">Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="e9341-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="e9341-116">Integrierte Rollen können nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="e9341-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="e9341-117">Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden.</span><span class="sxs-lookup"><span data-stu-id="e9341-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="e9341-118">Erstellen Sie eine benutzerdefinierte Rolle, wenn Sie eine Rolle definieren möchten, die beliebige der verfügbaren Ressourcen und Rollenberechtigungen in einer einzigen Rolle zusammenfasst.</span><span class="sxs-lookup"><span data-stu-id="e9341-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="e9341-119">Methoden</span><span class="sxs-lookup"><span data-stu-id="e9341-119">Methods</span></span>
|<span data-ttu-id="e9341-120">Methode</span><span class="sxs-lookup"><span data-stu-id="e9341-120">Method</span></span>|<span data-ttu-id="e9341-121">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e9341-121">Return Type</span></span>|<span data-ttu-id="e9341-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9341-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e9341-123">Auflisten von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="e9341-123">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="e9341-124">Sammlung von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e9341-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="e9341-125">Listet die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) auf.</span><span class="sxs-lookup"><span data-stu-id="e9341-125">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="e9341-126">Abrufen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="e9341-126">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="e9341-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e9341-127">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="e9341-128">Liest die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e9341-128">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="e9341-129">Erstellen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="e9341-129">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="e9341-130">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e9341-130">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="e9341-131">Erstellt neue Objekte des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e9341-131">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="e9341-132">Löschen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="e9341-132">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="e9341-133">Keiner</span><span class="sxs-lookup"><span data-stu-id="e9341-133">None</span></span>|<span data-ttu-id="e9341-134">Löscht Objekte des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e9341-134">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="e9341-135">Aktualisieren von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="e9341-135">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="e9341-136">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e9341-136">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="e9341-137">Aktualisiert die Eigenschaften von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e9341-137">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e9341-138">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e9341-138">Properties</span></span>
|<span data-ttu-id="e9341-139">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e9341-139">Property</span></span>|<span data-ttu-id="e9341-140">Typ</span><span class="sxs-lookup"><span data-stu-id="e9341-140">Type</span></span>|<span data-ttu-id="e9341-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9341-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9341-142">id</span><span class="sxs-lookup"><span data-stu-id="e9341-142">id</span></span>|<span data-ttu-id="e9341-143">String</span><span class="sxs-lookup"><span data-stu-id="e9341-143">String</span></span>|<span data-ttu-id="e9341-144">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e9341-144">Key of the entity.</span></span> <span data-ttu-id="e9341-145">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="e9341-145">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="e9341-146">displayName</span><span class="sxs-lookup"><span data-stu-id="e9341-146">displayName</span></span>|<span data-ttu-id="e9341-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e9341-147">String</span></span>|<span data-ttu-id="e9341-148">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="e9341-148">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="e9341-149">description</span><span class="sxs-lookup"><span data-stu-id="e9341-149">description</span></span>|<span data-ttu-id="e9341-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e9341-150">String</span></span>|<span data-ttu-id="e9341-151">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="e9341-151">Description of the Role definition.</span></span>|
|<span data-ttu-id="e9341-152">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e9341-152">permissions</span></span>|<span data-ttu-id="e9341-153">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="e9341-153">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="e9341-154">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="e9341-154">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e9341-155">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="e9341-155">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="e9341-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="e9341-156">rolePermissions</span></span>|<span data-ttu-id="e9341-157">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="e9341-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="e9341-158">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="e9341-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e9341-159">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="e9341-159">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="e9341-160">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e9341-160">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="e9341-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9341-161">Boolean</span></span>|<span data-ttu-id="e9341-162">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="e9341-162">Type of Role.</span></span> <span data-ttu-id="e9341-163">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="e9341-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="e9341-164">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="e9341-164">isBuiltIn</span></span>|<span data-ttu-id="e9341-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9341-165">Boolean</span></span>|<span data-ttu-id="e9341-166">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="e9341-166">Type of Role.</span></span> <span data-ttu-id="e9341-167">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="e9341-167">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="e9341-168">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="e9341-168">roleScopeTagIds</span></span>|<span data-ttu-id="e9341-169">String collection</span><span class="sxs-lookup"><span data-stu-id="e9341-169">String collection</span></span>|<span data-ttu-id="e9341-170">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="e9341-170">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9341-171">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e9341-171">Relationships</span></span>
|<span data-ttu-id="e9341-172">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e9341-172">Relationship</span></span>|<span data-ttu-id="e9341-173">Typ</span><span class="sxs-lookup"><span data-stu-id="e9341-173">Type</span></span>|<span data-ttu-id="e9341-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9341-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9341-175">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="e9341-175">roleAssignments</span></span>|<span data-ttu-id="e9341-176">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e9341-176">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="e9341-177">Liste der Rollenzuweisungen für die Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="e9341-177">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9341-178">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e9341-178">JSON Representation</span></span>
<span data-ttu-id="e9341-179">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e9341-179">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
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




