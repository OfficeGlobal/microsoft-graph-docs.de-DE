---
title: roleAssignment-Ressourcentyp
description: Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7cb3b07abc47224b2f96a35f4099d3a691b6c901
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825494"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="b8090-106">roleAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8090-106">roleAssignment resource type</span></span>

> <span data-ttu-id="b8090-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b8090-107">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8090-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8090-108">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8090-109">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b8090-109">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8090-110">Die Rollenzuweisungsressource.</span><span class="sxs-lookup"><span data-stu-id="b8090-110">The Role Assignment resource.</span></span> <span data-ttu-id="b8090-111">Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen.</span><span class="sxs-lookup"><span data-stu-id="b8090-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="b8090-112">Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben.</span><span class="sxs-lookup"><span data-stu-id="b8090-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="b8090-113">Dies gilt für benutzerdefinierte und integrierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="b8090-113">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="b8090-114">Methoden</span><span class="sxs-lookup"><span data-stu-id="b8090-114">Methods</span></span>
|<span data-ttu-id="b8090-115">Methode</span><span class="sxs-lookup"><span data-stu-id="b8090-115">Method</span></span>|<span data-ttu-id="b8090-116">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b8090-116">Return Type</span></span>|<span data-ttu-id="b8090-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8090-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8090-118">RoleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="b8090-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="b8090-119">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b8090-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="b8090-120">Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="b8090-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="b8090-121">RoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="b8090-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="b8090-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="b8090-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="b8090-123">Lesen von Eigenschaften und Beziehungen des [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8090-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="b8090-124">RoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="b8090-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="b8090-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="b8090-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="b8090-126">Erstellen eines neuen [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8090-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="b8090-127">RoleAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="b8090-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="b8090-128">Keine</span><span class="sxs-lookup"><span data-stu-id="b8090-128">None</span></span>|<span data-ttu-id="b8090-129">Löscht ein [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="b8090-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="b8090-130">RoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b8090-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="b8090-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="b8090-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="b8090-132">Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8090-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8090-133">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8090-133">Properties</span></span>
|<span data-ttu-id="b8090-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8090-134">Property</span></span>|<span data-ttu-id="b8090-135">Typ</span><span class="sxs-lookup"><span data-stu-id="b8090-135">Type</span></span>|<span data-ttu-id="b8090-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8090-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8090-137">id</span><span class="sxs-lookup"><span data-stu-id="b8090-137">id</span></span>|<span data-ttu-id="b8090-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8090-138">String</span></span>|<span data-ttu-id="b8090-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b8090-139">Key of the entity.</span></span> <span data-ttu-id="b8090-140">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="b8090-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b8090-141">displayName</span><span class="sxs-lookup"><span data-stu-id="b8090-141">displayName</span></span>|<span data-ttu-id="b8090-142">String</span><span class="sxs-lookup"><span data-stu-id="b8090-142">String</span></span>|<span data-ttu-id="b8090-143">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="b8090-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="b8090-144">description</span><span class="sxs-lookup"><span data-stu-id="b8090-144">description</span></span>|<span data-ttu-id="b8090-145">String</span><span class="sxs-lookup"><span data-stu-id="b8090-145">String</span></span>|<span data-ttu-id="b8090-146">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="b8090-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="b8090-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="b8090-147">scopeMembers</span></span>|<span data-ttu-id="b8090-148">String collection</span><span class="sxs-lookup"><span data-stu-id="b8090-148">String collection</span></span>|<span data-ttu-id="b8090-149">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="b8090-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b8090-150">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8090-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="b8090-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="b8090-151">scopeType</span></span>|[<span data-ttu-id="b8090-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="b8090-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="b8090-153">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="b8090-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="b8090-154">Standardtyp 'ResourceScope' ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="b8090-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="b8090-155">Für 'AllDevices', 'AllLicensedUsers' und 'AllDevicesAndLicensedUsers' sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="b8090-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="b8090-156">Mögliche Werte: sind `resourceScope`, `allDevices`, `allLicensedUsers` und `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="b8090-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="b8090-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b8090-157">resourceScopes</span></span>|<span data-ttu-id="b8090-158">String collection</span><span class="sxs-lookup"><span data-stu-id="b8090-158">String collection</span></span>|<span data-ttu-id="b8090-159">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="b8090-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b8090-160">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8090-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8090-161">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8090-161">Relationships</span></span>
|<span data-ttu-id="b8090-162">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b8090-162">Relationship</span></span>|<span data-ttu-id="b8090-163">Typ</span><span class="sxs-lookup"><span data-stu-id="b8090-163">Type</span></span>|<span data-ttu-id="b8090-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8090-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8090-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b8090-165">roleDefinition</span></span>|[<span data-ttu-id="b8090-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b8090-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="b8090-167">Die Rollendefinition, in der diese Zuweisung enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="b8090-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8090-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8090-168">JSON Representation</span></span>
<span data-ttu-id="b8090-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8090-169">Here is a JSON representation of the resource.</span></span>
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





