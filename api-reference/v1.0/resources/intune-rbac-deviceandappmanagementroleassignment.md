---
title: deviceAndAppManagementRoleAssignment-Ressourcentyp
description: Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bfbb4e3b51f56e447ba69caefbf2b0b5226a5d4f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264085"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="5246c-106">deviceAndAppManagementRoleAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5246c-106">deviceAndAppManagementRoleAssignment resource type</span></span>

> <span data-ttu-id="5246c-107">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5246c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5246c-108">Die Rollenzuweisungsressource.</span><span class="sxs-lookup"><span data-stu-id="5246c-108">The Role Assignment resource.</span></span> <span data-ttu-id="5246c-109">Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen.</span><span class="sxs-lookup"><span data-stu-id="5246c-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="5246c-110">Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben.</span><span class="sxs-lookup"><span data-stu-id="5246c-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="5246c-111">Dies gilt für benutzerdefinierte und integrierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="5246c-111">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="5246c-112">Erbt von [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5246c-112">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5246c-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="5246c-113">Methods</span></span>
|<span data-ttu-id="5246c-114">Methode</span><span class="sxs-lookup"><span data-stu-id="5246c-114">Method</span></span>|<span data-ttu-id="5246c-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5246c-115">Return Type</span></span>|<span data-ttu-id="5246c-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5246c-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5246c-117">deviceAndAppManagementRoleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="5246c-117">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="5246c-118">[DeviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5246c-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="5246c-119">Auflisten von Eigenschaften und Beziehungen der [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="5246c-119">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="5246c-120">DeviceAndAppManagementRoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="5246c-120">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="5246c-121">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5246c-121">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="5246c-122">Lesen von Eigenschaften und Beziehungen des [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5246c-122">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="5246c-123">DeviceAndAppManagementRoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="5246c-123">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="5246c-124">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5246c-124">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="5246c-125">Erstellen eines neuen [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5246c-125">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="5246c-126">DeviceAndAppManagementRoleAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="5246c-126">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="5246c-127">Keine</span><span class="sxs-lookup"><span data-stu-id="5246c-127">None</span></span>|<span data-ttu-id="5246c-128">Löscht ein [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="5246c-128">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="5246c-129">DeviceAndAppManagementRoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5246c-129">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="5246c-130">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5246c-130">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="5246c-131">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5246c-131">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5246c-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5246c-132">Properties</span></span>
|<span data-ttu-id="5246c-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5246c-133">Property</span></span>|<span data-ttu-id="5246c-134">Typ</span><span class="sxs-lookup"><span data-stu-id="5246c-134">Type</span></span>|<span data-ttu-id="5246c-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5246c-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5246c-136">id</span><span class="sxs-lookup"><span data-stu-id="5246c-136">id</span></span>|<span data-ttu-id="5246c-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5246c-137">String</span></span>|<span data-ttu-id="5246c-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5246c-138">Key of the entity.</span></span> <span data-ttu-id="5246c-139">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="5246c-139">This is read-only and automatically generated.</span></span> <span data-ttu-id="5246c-140">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5246c-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5246c-141">displayName</span><span class="sxs-lookup"><span data-stu-id="5246c-141">displayName</span></span>|<span data-ttu-id="5246c-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5246c-142">String</span></span>|<span data-ttu-id="5246c-143">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="5246c-143">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="5246c-144">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5246c-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5246c-145">description</span><span class="sxs-lookup"><span data-stu-id="5246c-145">description</span></span>|<span data-ttu-id="5246c-146">String</span><span class="sxs-lookup"><span data-stu-id="5246c-146">String</span></span>|<span data-ttu-id="5246c-147">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="5246c-147">Description of the Role Assignment.</span></span> <span data-ttu-id="5246c-148">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5246c-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5246c-149">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="5246c-149">resourceScopes</span></span>|<span data-ttu-id="5246c-150">String collection</span><span class="sxs-lookup"><span data-stu-id="5246c-150">String collection</span></span>|<span data-ttu-id="5246c-151">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="5246c-151">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="5246c-152">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5246c-152">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="5246c-153">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5246c-153">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5246c-154">members</span><span class="sxs-lookup"><span data-stu-id="5246c-154">members</span></span>|<span data-ttu-id="5246c-155">String collection</span><span class="sxs-lookup"><span data-stu-id="5246c-155">String collection</span></span>|<span data-ttu-id="5246c-156">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="5246c-156">The list of ids of role member security groups.</span></span> <span data-ttu-id="5246c-157">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5246c-157">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5246c-158">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5246c-158">Relationships</span></span>
|<span data-ttu-id="5246c-159">Beziehung</span><span class="sxs-lookup"><span data-stu-id="5246c-159">Relationship</span></span>|<span data-ttu-id="5246c-160">Typ</span><span class="sxs-lookup"><span data-stu-id="5246c-160">Type</span></span>|<span data-ttu-id="5246c-161">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5246c-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5246c-162">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5246c-162">roleDefinition</span></span>|[<span data-ttu-id="5246c-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5246c-163">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="5246c-164">Die Rollendefinition, in der diese Zuweisung enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="5246c-164">Role definition this assignment is part of.</span></span> <span data-ttu-id="5246c-165">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5246c-165">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5246c-166">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5246c-166">JSON Representation</span></span>
<span data-ttu-id="5246c-167">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5246c-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```



