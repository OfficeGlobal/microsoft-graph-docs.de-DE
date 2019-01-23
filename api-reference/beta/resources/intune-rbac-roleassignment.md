---
title: roleAssignment-Ressourcentyp
description: Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 11fc37502fa017494ff884cb70f0006277a42600
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415124"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="1f108-106">roleAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1f108-106">roleAssignment resource type</span></span>

> <span data-ttu-id="1f108-107">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1f108-107">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1f108-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f108-108">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f108-109">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f108-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f108-110">Die Rollenzuweisungsressource.</span><span class="sxs-lookup"><span data-stu-id="1f108-110">The Role Assignment resource.</span></span> <span data-ttu-id="1f108-111">Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen.</span><span class="sxs-lookup"><span data-stu-id="1f108-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="1f108-112">Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben.</span><span class="sxs-lookup"><span data-stu-id="1f108-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="1f108-113">Dies gilt für benutzerdefinierte und integrierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="1f108-113">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="1f108-114">Methoden</span><span class="sxs-lookup"><span data-stu-id="1f108-114">Methods</span></span>
|<span data-ttu-id="1f108-115">Methode</span><span class="sxs-lookup"><span data-stu-id="1f108-115">Method</span></span>|<span data-ttu-id="1f108-116">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1f108-116">Return Type</span></span>|<span data-ttu-id="1f108-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f108-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1f108-118">RoleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="1f108-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="1f108-119">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1f108-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="1f108-120">Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="1f108-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="1f108-121">RoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="1f108-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="1f108-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="1f108-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="1f108-123">Lesen von Eigenschaften und Beziehungen des [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f108-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="1f108-124">RoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="1f108-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="1f108-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="1f108-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="1f108-126">Erstellen eines neuen [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f108-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="1f108-127">RoleAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="1f108-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="1f108-128">Keine</span><span class="sxs-lookup"><span data-stu-id="1f108-128">None</span></span>|<span data-ttu-id="1f108-129">Löscht ein [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="1f108-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="1f108-130">RoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1f108-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="1f108-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="1f108-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="1f108-132">Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f108-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f108-133">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1f108-133">Properties</span></span>
|<span data-ttu-id="1f108-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f108-134">Property</span></span>|<span data-ttu-id="1f108-135">Typ</span><span class="sxs-lookup"><span data-stu-id="1f108-135">Type</span></span>|<span data-ttu-id="1f108-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f108-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f108-137">id</span><span class="sxs-lookup"><span data-stu-id="1f108-137">id</span></span>|<span data-ttu-id="1f108-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f108-138">String</span></span>|<span data-ttu-id="1f108-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1f108-139">Key of the entity.</span></span> <span data-ttu-id="1f108-140">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="1f108-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="1f108-141">displayName</span><span class="sxs-lookup"><span data-stu-id="1f108-141">displayName</span></span>|<span data-ttu-id="1f108-142">String</span><span class="sxs-lookup"><span data-stu-id="1f108-142">String</span></span>|<span data-ttu-id="1f108-143">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="1f108-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="1f108-144">description</span><span class="sxs-lookup"><span data-stu-id="1f108-144">description</span></span>|<span data-ttu-id="1f108-145">String</span><span class="sxs-lookup"><span data-stu-id="1f108-145">String</span></span>|<span data-ttu-id="1f108-146">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="1f108-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="1f108-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="1f108-147">scopeMembers</span></span>|<span data-ttu-id="1f108-148">String collection</span><span class="sxs-lookup"><span data-stu-id="1f108-148">String collection</span></span>|<span data-ttu-id="1f108-149">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="1f108-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="1f108-150">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1f108-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="1f108-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="1f108-151">scopeType</span></span>|[<span data-ttu-id="1f108-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="1f108-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="1f108-153">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="1f108-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="1f108-154">Standardtyp 'ResourceScope' ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="1f108-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="1f108-155">Für 'AllDevices', 'AllLicensedUsers' und 'AllDevicesAndLicensedUsers' sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="1f108-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="1f108-156">Mögliche Werte: sind `resourceScope`, `allDevices`, `allLicensedUsers` und `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="1f108-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="1f108-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="1f108-157">resourceScopes</span></span>|<span data-ttu-id="1f108-158">String collection</span><span class="sxs-lookup"><span data-stu-id="1f108-158">String collection</span></span>|<span data-ttu-id="1f108-159">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="1f108-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="1f108-160">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1f108-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f108-161">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1f108-161">Relationships</span></span>
|<span data-ttu-id="1f108-162">Beziehung</span><span class="sxs-lookup"><span data-stu-id="1f108-162">Relationship</span></span>|<span data-ttu-id="1f108-163">Typ</span><span class="sxs-lookup"><span data-stu-id="1f108-163">Type</span></span>|<span data-ttu-id="1f108-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f108-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f108-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1f108-165">roleDefinition</span></span>|[<span data-ttu-id="1f108-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1f108-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="1f108-167">Die Rollendefinition, in der diese Zuweisung enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="1f108-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f108-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1f108-168">JSON Representation</span></span>
<span data-ttu-id="1f108-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1f108-169">Here is a JSON representation of the resource.</span></span>
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




