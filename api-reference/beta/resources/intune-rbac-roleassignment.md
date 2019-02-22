---
title: roleAssignment-Ressourcentyp
description: Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71ca364b74e2f7df672fee1880343c0f2372500d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162937"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="766b1-106">roleAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="766b1-106">roleAssignment resource type</span></span>

> <span data-ttu-id="766b1-107">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="766b1-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="766b1-108">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="766b1-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="766b1-109">Die Rollenzuweisungsressource.</span><span class="sxs-lookup"><span data-stu-id="766b1-109">The Role Assignment resource.</span></span> <span data-ttu-id="766b1-110">Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen.</span><span class="sxs-lookup"><span data-stu-id="766b1-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="766b1-111">Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben.</span><span class="sxs-lookup"><span data-stu-id="766b1-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="766b1-112">Dies gilt für benutzerdefinierte und integrierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="766b1-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="766b1-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="766b1-113">Methods</span></span>
|<span data-ttu-id="766b1-114">Methode</span><span class="sxs-lookup"><span data-stu-id="766b1-114">Method</span></span>|<span data-ttu-id="766b1-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="766b1-115">Return Type</span></span>|<span data-ttu-id="766b1-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="766b1-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="766b1-117">RoleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="766b1-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="766b1-118">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="766b1-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="766b1-119">Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="766b1-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="766b1-120">RoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="766b1-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="766b1-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="766b1-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="766b1-122">Lesen von Eigenschaften und Beziehungen des [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="766b1-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="766b1-123">RoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="766b1-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="766b1-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="766b1-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="766b1-125">Erstellen eines neuen [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="766b1-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="766b1-126">RoleAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="766b1-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="766b1-127">Keine</span><span class="sxs-lookup"><span data-stu-id="766b1-127">None</span></span>|<span data-ttu-id="766b1-128">Löscht ein [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="766b1-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="766b1-129">RoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="766b1-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="766b1-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="766b1-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="766b1-131">Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="766b1-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="766b1-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="766b1-132">Properties</span></span>
|<span data-ttu-id="766b1-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="766b1-133">Property</span></span>|<span data-ttu-id="766b1-134">Typ</span><span class="sxs-lookup"><span data-stu-id="766b1-134">Type</span></span>|<span data-ttu-id="766b1-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="766b1-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="766b1-136">id</span><span class="sxs-lookup"><span data-stu-id="766b1-136">id</span></span>|<span data-ttu-id="766b1-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="766b1-137">String</span></span>|<span data-ttu-id="766b1-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="766b1-138">Key of the entity.</span></span> <span data-ttu-id="766b1-139">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="766b1-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="766b1-140">displayName</span><span class="sxs-lookup"><span data-stu-id="766b1-140">displayName</span></span>|<span data-ttu-id="766b1-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="766b1-141">String</span></span>|<span data-ttu-id="766b1-142">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="766b1-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="766b1-143">description</span><span class="sxs-lookup"><span data-stu-id="766b1-143">description</span></span>|<span data-ttu-id="766b1-144">String</span><span class="sxs-lookup"><span data-stu-id="766b1-144">String</span></span>|<span data-ttu-id="766b1-145">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="766b1-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="766b1-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="766b1-146">scopeMembers</span></span>|<span data-ttu-id="766b1-147">String collection</span><span class="sxs-lookup"><span data-stu-id="766b1-147">String collection</span></span>|<span data-ttu-id="766b1-148">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="766b1-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="766b1-149">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="766b1-149">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="766b1-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="766b1-150">scopeType</span></span>|[<span data-ttu-id="766b1-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="766b1-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="766b1-152">Gibt den Typ des Bereichs für eine Rollenzuweisung an.</span><span class="sxs-lookup"><span data-stu-id="766b1-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="766b1-153">Der Standardtyp "ResourceScope" ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="766b1-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="766b1-154">Für "allDevices", "AllLicensedUsers" und "AllDevicesAndLicensedUsers" sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="766b1-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="766b1-155">Mögliche Werte: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="766b1-155">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="766b1-156">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="766b1-156">resourceScopes</span></span>|<span data-ttu-id="766b1-157">String collection</span><span class="sxs-lookup"><span data-stu-id="766b1-157">String collection</span></span>|<span data-ttu-id="766b1-158">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="766b1-158">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="766b1-159">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="766b1-159">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="766b1-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="766b1-160">Relationships</span></span>
|<span data-ttu-id="766b1-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="766b1-161">Relationship</span></span>|<span data-ttu-id="766b1-162">Typ</span><span class="sxs-lookup"><span data-stu-id="766b1-162">Type</span></span>|<span data-ttu-id="766b1-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="766b1-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="766b1-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="766b1-164">roleDefinition</span></span>|[<span data-ttu-id="766b1-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="766b1-165">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="766b1-166">Die Rollendefinition, in der diese Zuweisung enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="766b1-166">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="766b1-167">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="766b1-167">JSON Representation</span></span>
<span data-ttu-id="766b1-168">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="766b1-168">Here is a JSON representation of the resource.</span></span>
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




