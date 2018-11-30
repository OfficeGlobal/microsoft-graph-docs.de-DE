---
title: Ressourcentyp „roleDefinition“
description: 'Die Rollendefinitionsressource. Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune. In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert. Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen. Integrierte Rollen können nicht geändert werden. Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden. Erstellen Sie benutzerdefinierte Rollen, wenn Sie eine Rolle definieren möchten, in der beliebige der verfügbaren Ressourcen und Rollenberechtigungen kombiniert werden können.'
ms.openlocfilehash: 872985dd3ba99d4afbdbee3b6bc37055f3800020
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065747"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="7a330-109">Ressourcentyp „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="7a330-109">roleDefinition resource type</span></span>

> <span data-ttu-id="7a330-110">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7a330-110">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a330-111">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a330-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a330-112">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7a330-112">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a330-113">Die Rollendefinitionsressource.</span><span class="sxs-lookup"><span data-stu-id="7a330-113">The Role Definition resource.</span></span> <span data-ttu-id="7a330-114">Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune.</span><span class="sxs-lookup"><span data-stu-id="7a330-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="7a330-115">In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert.</span><span class="sxs-lookup"><span data-stu-id="7a330-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="7a330-116">Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="7a330-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="7a330-117">Integrierte Rollen können nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="7a330-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="7a330-118">Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden.</span><span class="sxs-lookup"><span data-stu-id="7a330-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="7a330-119">Erstellen Sie eine benutzerdefinierte Rolle, wenn Sie eine Rolle definieren möchten, die beliebige der verfügbaren Ressourcen und Rollenberechtigungen in einer einzigen Rolle zusammenfasst.</span><span class="sxs-lookup"><span data-stu-id="7a330-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="7a330-120">Methoden</span><span class="sxs-lookup"><span data-stu-id="7a330-120">Methods</span></span>
|<span data-ttu-id="7a330-121">Methode</span><span class="sxs-lookup"><span data-stu-id="7a330-121">Method</span></span>|<span data-ttu-id="7a330-122">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7a330-122">Return Type</span></span>|<span data-ttu-id="7a330-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a330-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7a330-124">Auflisten von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="7a330-124">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="7a330-125">Sammlung von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7a330-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="7a330-126">Listet die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) auf.</span><span class="sxs-lookup"><span data-stu-id="7a330-126">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="7a330-127">Abrufen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="7a330-127">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="7a330-128">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7a330-128">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="7a330-129">Liest die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7a330-129">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="7a330-130">Erstellen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="7a330-130">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="7a330-131">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7a330-131">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="7a330-132">Erstellt neue Objekte des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7a330-132">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="7a330-133">Löschen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="7a330-133">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="7a330-134">Keiner</span><span class="sxs-lookup"><span data-stu-id="7a330-134">None</span></span>|<span data-ttu-id="7a330-135">Löscht Objekte des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7a330-135">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="7a330-136">Aktualisieren von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="7a330-136">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="7a330-137">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7a330-137">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="7a330-138">Aktualisiert die Eigenschaften von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7a330-138">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a330-139">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7a330-139">Properties</span></span>
|<span data-ttu-id="7a330-140">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7a330-140">Property</span></span>|<span data-ttu-id="7a330-141">Typ</span><span class="sxs-lookup"><span data-stu-id="7a330-141">Type</span></span>|<span data-ttu-id="7a330-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a330-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a330-143">id</span><span class="sxs-lookup"><span data-stu-id="7a330-143">id</span></span>|<span data-ttu-id="7a330-144">String</span><span class="sxs-lookup"><span data-stu-id="7a330-144">String</span></span>|<span data-ttu-id="7a330-145">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7a330-145">Key of the entity.</span></span> <span data-ttu-id="7a330-146">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="7a330-146">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="7a330-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7a330-147">displayName</span></span>|<span data-ttu-id="7a330-148">String</span><span class="sxs-lookup"><span data-stu-id="7a330-148">String</span></span>|<span data-ttu-id="7a330-149">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="7a330-149">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="7a330-150">description</span><span class="sxs-lookup"><span data-stu-id="7a330-150">description</span></span>|<span data-ttu-id="7a330-151">String</span><span class="sxs-lookup"><span data-stu-id="7a330-151">String</span></span>|<span data-ttu-id="7a330-152">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="7a330-152">Description of the Role definition.</span></span>|
|<span data-ttu-id="7a330-153">permissions</span><span class="sxs-lookup"><span data-stu-id="7a330-153">permissions</span></span>|<span data-ttu-id="7a330-154">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="7a330-154">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="7a330-155">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="7a330-155">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7a330-156">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="7a330-156">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="7a330-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="7a330-157">rolePermissions</span></span>|<span data-ttu-id="7a330-158">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="7a330-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="7a330-159">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="7a330-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7a330-160">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="7a330-160">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="7a330-161">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7a330-161">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="7a330-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a330-162">Boolean</span></span>|<span data-ttu-id="7a330-163">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="7a330-163">Type of Role.</span></span> <span data-ttu-id="7a330-164">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="7a330-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="7a330-165">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="7a330-165">isBuiltIn</span></span>|<span data-ttu-id="7a330-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a330-166">Boolean</span></span>|<span data-ttu-id="7a330-167">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="7a330-167">Type of Role.</span></span> <span data-ttu-id="7a330-168">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="7a330-168">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a330-169">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7a330-169">Relationships</span></span>
|<span data-ttu-id="7a330-170">Beziehung</span><span class="sxs-lookup"><span data-stu-id="7a330-170">Relationship</span></span>|<span data-ttu-id="7a330-171">Typ</span><span class="sxs-lookup"><span data-stu-id="7a330-171">Type</span></span>|<span data-ttu-id="7a330-172">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a330-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a330-173">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="7a330-173">roleAssignments</span></span>|<span data-ttu-id="7a330-174">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7a330-174">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="7a330-175">Liste der Rollenzuweisungen für die Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="7a330-175">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a330-176">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7a330-176">JSON Representation</span></span>
<span data-ttu-id="7a330-177">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7a330-177">Here is a JSON representation of the resource.</span></span>
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
  "isBuiltIn": true
}
```





