---
title: roleAssignment-Ressourcentyp
description: Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32527fad8db54f865f054f04400897e51638e5c2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258429"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="72dfa-106">roleAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="72dfa-106">roleAssignment resource type</span></span>

> <span data-ttu-id="72dfa-107">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="72dfa-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72dfa-108">Die Rollenzuweisungsressource.</span><span class="sxs-lookup"><span data-stu-id="72dfa-108">The Role Assignment resource.</span></span> <span data-ttu-id="72dfa-109">Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen.</span><span class="sxs-lookup"><span data-stu-id="72dfa-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="72dfa-110">Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben.</span><span class="sxs-lookup"><span data-stu-id="72dfa-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="72dfa-111">Dies gilt für benutzerdefinierte und integrierte Rollen.</span><span class="sxs-lookup"><span data-stu-id="72dfa-111">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="72dfa-112">Methoden</span><span class="sxs-lookup"><span data-stu-id="72dfa-112">Methods</span></span>
|<span data-ttu-id="72dfa-113">Methode</span><span class="sxs-lookup"><span data-stu-id="72dfa-113">Method</span></span>|<span data-ttu-id="72dfa-114">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="72dfa-114">Return Type</span></span>|<span data-ttu-id="72dfa-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72dfa-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="72dfa-116">RoleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="72dfa-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="72dfa-117">Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="72dfa-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="72dfa-118">Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="72dfa-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="72dfa-119">RoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="72dfa-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="72dfa-120">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="72dfa-120">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="72dfa-121">Lesen von Eigenschaften und Beziehungen des [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="72dfa-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="72dfa-122">RoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="72dfa-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="72dfa-123">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="72dfa-123">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="72dfa-124">Erstellen eines neuen [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="72dfa-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="72dfa-125">RoleAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="72dfa-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="72dfa-126">Keine</span><span class="sxs-lookup"><span data-stu-id="72dfa-126">None</span></span>|<span data-ttu-id="72dfa-127">Löscht ein [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="72dfa-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="72dfa-128">RoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="72dfa-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="72dfa-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="72dfa-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="72dfa-130">Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="72dfa-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="72dfa-131">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="72dfa-131">Properties</span></span>
|<span data-ttu-id="72dfa-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="72dfa-132">Property</span></span>|<span data-ttu-id="72dfa-133">Typ</span><span class="sxs-lookup"><span data-stu-id="72dfa-133">Type</span></span>|<span data-ttu-id="72dfa-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72dfa-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72dfa-135">id</span><span class="sxs-lookup"><span data-stu-id="72dfa-135">id</span></span>|<span data-ttu-id="72dfa-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72dfa-136">String</span></span>|<span data-ttu-id="72dfa-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="72dfa-137">Key of the entity.</span></span> <span data-ttu-id="72dfa-138">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="72dfa-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="72dfa-139">displayName</span><span class="sxs-lookup"><span data-stu-id="72dfa-139">displayName</span></span>|<span data-ttu-id="72dfa-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72dfa-140">String</span></span>|<span data-ttu-id="72dfa-141">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="72dfa-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="72dfa-142">description</span><span class="sxs-lookup"><span data-stu-id="72dfa-142">description</span></span>|<span data-ttu-id="72dfa-143">String</span><span class="sxs-lookup"><span data-stu-id="72dfa-143">String</span></span>|<span data-ttu-id="72dfa-144">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="72dfa-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="72dfa-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="72dfa-145">resourceScopes</span></span>|<span data-ttu-id="72dfa-146">String collection</span><span class="sxs-lookup"><span data-stu-id="72dfa-146">String collection</span></span>|<span data-ttu-id="72dfa-147">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="72dfa-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="72dfa-148">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="72dfa-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72dfa-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="72dfa-149">Relationships</span></span>
|<span data-ttu-id="72dfa-150">Beziehung</span><span class="sxs-lookup"><span data-stu-id="72dfa-150">Relationship</span></span>|<span data-ttu-id="72dfa-151">Typ</span><span class="sxs-lookup"><span data-stu-id="72dfa-151">Type</span></span>|<span data-ttu-id="72dfa-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72dfa-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72dfa-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="72dfa-153">roleDefinition</span></span>|[<span data-ttu-id="72dfa-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="72dfa-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="72dfa-155">Die Rollendefinition, in der diese Zuweisung enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="72dfa-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72dfa-156">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="72dfa-156">JSON Representation</span></span>
<span data-ttu-id="72dfa-157">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="72dfa-157">Here is a JSON representation of the resource.</span></span>
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



