---
title: Ressourcentyp „roleDefinition“
description: 'Die Rollendefinitionsressource. Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune. In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert. Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen. Integrierte Rollen können nicht geändert werden. Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden. Erstellen Sie benutzerdefinierte Rollen, wenn Sie eine Rolle definieren möchten, in der beliebige der verfügbaren Ressourcen und Rollenberechtigungen kombiniert werden können.'
ms.openlocfilehash: 15be13c0a893ed0cdc7b77b47591cc28d32c9889
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018094"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="54e6b-109">Ressourcentyp „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="54e6b-109">roleDefinition resource type</span></span>

> <span data-ttu-id="54e6b-110">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="54e6b-110">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54e6b-111">Die Rollendefinitionsressource.</span><span class="sxs-lookup"><span data-stu-id="54e6b-111">The Role Definition resource.</span></span> <span data-ttu-id="54e6b-112">Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune.</span><span class="sxs-lookup"><span data-stu-id="54e6b-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="54e6b-113">In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert.</span><span class="sxs-lookup"><span data-stu-id="54e6b-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="54e6b-114">Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="54e6b-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="54e6b-115">Integrierte Rollen können nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="54e6b-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="54e6b-116">Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden.</span><span class="sxs-lookup"><span data-stu-id="54e6b-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="54e6b-117">Erstellen Sie eine benutzerdefinierte Rolle, wenn Sie eine Rolle definieren möchten, die beliebige der verfügbaren Ressourcen und Rollenberechtigungen in einer einzigen Rolle zusammenfasst.</span><span class="sxs-lookup"><span data-stu-id="54e6b-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="54e6b-118">Methoden</span><span class="sxs-lookup"><span data-stu-id="54e6b-118">Methods</span></span>
|<span data-ttu-id="54e6b-119">Methode</span><span class="sxs-lookup"><span data-stu-id="54e6b-119">Method</span></span>|<span data-ttu-id="54e6b-120">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="54e6b-120">Return Type</span></span>|<span data-ttu-id="54e6b-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54e6b-121">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="54e6b-122">Auflisten von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="54e6b-122">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="54e6b-123">Sammlung von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="54e6b-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="54e6b-124">Listet die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) auf.</span><span class="sxs-lookup"><span data-stu-id="54e6b-124">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="54e6b-125">Abrufen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="54e6b-125">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="54e6b-126">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="54e6b-126">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="54e6b-127">Liest die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="54e6b-127">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="54e6b-128">Erstellen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="54e6b-128">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="54e6b-129">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="54e6b-129">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="54e6b-130">Erstellt neue Objekte des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="54e6b-130">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="54e6b-131">Löschen von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="54e6b-131">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="54e6b-132">Keiner</span><span class="sxs-lookup"><span data-stu-id="54e6b-132">None</span></span>|<span data-ttu-id="54e6b-133">Löscht Objekte des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="54e6b-133">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="54e6b-134">Aktualisieren von „roleDefinition“</span><span class="sxs-lookup"><span data-stu-id="54e6b-134">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="54e6b-135">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="54e6b-135">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="54e6b-136">Aktualisiert die Eigenschaften von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="54e6b-136">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="54e6b-137">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="54e6b-137">Properties</span></span>
|<span data-ttu-id="54e6b-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54e6b-138">Property</span></span>|<span data-ttu-id="54e6b-139">Typ</span><span class="sxs-lookup"><span data-stu-id="54e6b-139">Type</span></span>|<span data-ttu-id="54e6b-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54e6b-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54e6b-141">id</span><span class="sxs-lookup"><span data-stu-id="54e6b-141">id</span></span>|<span data-ttu-id="54e6b-142">String</span><span class="sxs-lookup"><span data-stu-id="54e6b-142">String</span></span>|<span data-ttu-id="54e6b-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="54e6b-143">Key of the entity.</span></span> <span data-ttu-id="54e6b-144">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="54e6b-144">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="54e6b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="54e6b-145">displayName</span></span>|<span data-ttu-id="54e6b-146">String</span><span class="sxs-lookup"><span data-stu-id="54e6b-146">String</span></span>|<span data-ttu-id="54e6b-147">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="54e6b-147">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="54e6b-148">description</span><span class="sxs-lookup"><span data-stu-id="54e6b-148">description</span></span>|<span data-ttu-id="54e6b-149">String</span><span class="sxs-lookup"><span data-stu-id="54e6b-149">String</span></span>|<span data-ttu-id="54e6b-150">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="54e6b-150">Description of the Role definition.</span></span>|
|<span data-ttu-id="54e6b-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="54e6b-151">rolePermissions</span></span>|<span data-ttu-id="54e6b-152">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="54e6b-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="54e6b-153">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="54e6b-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="54e6b-154">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="54e6b-154">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="54e6b-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="54e6b-155">isBuiltIn</span></span>|<span data-ttu-id="54e6b-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="54e6b-156">Boolean</span></span>|<span data-ttu-id="54e6b-157">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="54e6b-157">Type of Role.</span></span> <span data-ttu-id="54e6b-158">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="54e6b-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54e6b-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="54e6b-159">Relationships</span></span>
|<span data-ttu-id="54e6b-160">Beziehung</span><span class="sxs-lookup"><span data-stu-id="54e6b-160">Relationship</span></span>|<span data-ttu-id="54e6b-161">Typ</span><span class="sxs-lookup"><span data-stu-id="54e6b-161">Type</span></span>|<span data-ttu-id="54e6b-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54e6b-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54e6b-163">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="54e6b-163">roleAssignments</span></span>|<span data-ttu-id="54e6b-164">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="54e6b-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="54e6b-165">Liste der Rollenzuweisungen für die Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="54e6b-165">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54e6b-166">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="54e6b-166">JSON Representation</span></span>
<span data-ttu-id="54e6b-167">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="54e6b-167">Here is a JSON representation of the resource.</span></span>
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
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```


