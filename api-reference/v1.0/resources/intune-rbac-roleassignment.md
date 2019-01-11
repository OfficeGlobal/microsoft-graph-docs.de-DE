---
title: roleAssignment-Ressourcentyp
description: Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e8506b87975b69f90cf561e776e557bb472f1ffd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846151"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="fdb2b-106">roleAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fdb2b-106">roleAssignment resource type</span></span>

> <span data-ttu-id="fdb2b-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdb2b-108">Die Rollenzuweisungsressource.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-108">The Role Assignment resource.</span></span> <span data-ttu-id="fdb2b-109">Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="fdb2b-110">Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="fdb2b-111">Dies gilt für benutzerdefinierte und integrierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-111">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="fdb2b-112">Methoden</span><span class="sxs-lookup"><span data-stu-id="fdb2b-112">Methods</span></span>
|<span data-ttu-id="fdb2b-113">Methode</span><span class="sxs-lookup"><span data-stu-id="fdb2b-113">Method</span></span>|<span data-ttu-id="fdb2b-114">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fdb2b-114">Return Type</span></span>|<span data-ttu-id="fdb2b-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdb2b-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fdb2b-116">RoleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="fdb2b-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="fdb2b-117">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fdb2b-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="fdb2b-118">Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="fdb2b-119">RoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="fdb2b-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="fdb2b-120">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="fdb2b-120">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="fdb2b-121">Lesen von Eigenschaften und Beziehungen des [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="fdb2b-122">RoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="fdb2b-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="fdb2b-123">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="fdb2b-123">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="fdb2b-124">Erstellen eines neuen [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="fdb2b-125">RoleAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="fdb2b-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="fdb2b-126">Keine</span><span class="sxs-lookup"><span data-stu-id="fdb2b-126">None</span></span>|<span data-ttu-id="fdb2b-127">Löscht ein [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="fdb2b-128">RoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fdb2b-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="fdb2b-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="fdb2b-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="fdb2b-130">Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fdb2b-131">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fdb2b-131">Properties</span></span>
|<span data-ttu-id="fdb2b-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fdb2b-132">Property</span></span>|<span data-ttu-id="fdb2b-133">Typ</span><span class="sxs-lookup"><span data-stu-id="fdb2b-133">Type</span></span>|<span data-ttu-id="fdb2b-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdb2b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdb2b-135">id</span><span class="sxs-lookup"><span data-stu-id="fdb2b-135">id</span></span>|<span data-ttu-id="fdb2b-136">String</span><span class="sxs-lookup"><span data-stu-id="fdb2b-136">String</span></span>|<span data-ttu-id="fdb2b-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fdb2b-137">Key of the entity.</span></span> <span data-ttu-id="fdb2b-138">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="fdb2b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="fdb2b-139">displayName</span></span>|<span data-ttu-id="fdb2b-140">String</span><span class="sxs-lookup"><span data-stu-id="fdb2b-140">String</span></span>|<span data-ttu-id="fdb2b-141">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="fdb2b-142">description</span><span class="sxs-lookup"><span data-stu-id="fdb2b-142">description</span></span>|<span data-ttu-id="fdb2b-143">String</span><span class="sxs-lookup"><span data-stu-id="fdb2b-143">String</span></span>|<span data-ttu-id="fdb2b-144">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="fdb2b-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="fdb2b-145">resourceScopes</span></span>|<span data-ttu-id="fdb2b-146">String collection</span><span class="sxs-lookup"><span data-stu-id="fdb2b-146">String collection</span></span>|<span data-ttu-id="fdb2b-147">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fdb2b-148">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdb2b-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fdb2b-149">Relationships</span></span>
|<span data-ttu-id="fdb2b-150">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fdb2b-150">Relationship</span></span>|<span data-ttu-id="fdb2b-151">Typ</span><span class="sxs-lookup"><span data-stu-id="fdb2b-151">Type</span></span>|<span data-ttu-id="fdb2b-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdb2b-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdb2b-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="fdb2b-153">roleDefinition</span></span>|[<span data-ttu-id="fdb2b-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="fdb2b-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="fdb2b-155">Die Rollendefinition, in der diese Zuweisung enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdb2b-156">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fdb2b-156">JSON Representation</span></span>
<span data-ttu-id="fdb2b-157">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fdb2b-157">Here is a JSON representation of the resource.</span></span>
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
  "resourceScopes": [
    "String"
  ]
}
```



