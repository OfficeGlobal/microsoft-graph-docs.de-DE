---
title: Ressourcentyp privilegedRole
description: 'Stellt eine Azure AD-Administratorrolle z. B.: **globaler Administrator, Abrechnungsadministrator, Dienstadministrator, Benutzer-Administrator, Kennwort-Administrator**usw..'
ms.openlocfilehash: 0c04ab9de13732e4ac9eecb943a10945bec59d02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059079"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="9bc29-103">Ressourcentyp privilegedRole</span><span class="sxs-lookup"><span data-stu-id="9bc29-103">privilegedRole resource type</span></span>

> <span data-ttu-id="9bc29-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9bc29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bc29-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9bc29-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9bc29-106">Stellt eine Azure AD-Administratorrolle z. B.: **globaler Administrator, Abrechnungsadministrator, Dienstadministrator, Benutzer-Administrator, Kennwort-Administrator**usw..</span><span class="sxs-lookup"><span data-stu-id="9bc29-106">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="9bc29-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="9bc29-107">Methods</span></span>

| <span data-ttu-id="9bc29-108">Methode</span><span class="sxs-lookup"><span data-stu-id="9bc29-108">Method</span></span>           | <span data-ttu-id="9bc29-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9bc29-109">Return Type</span></span>    |<span data-ttu-id="9bc29-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bc29-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9bc29-111">Objekte in der Liste privilegedRole</span><span class="sxs-lookup"><span data-stu-id="9bc29-111">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="9bc29-112">[PrivilegedRole](privilegedrole.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9bc29-112">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="9bc29-113">Ruft die Auflistung der PrivilegedRole.</span><span class="sxs-lookup"><span data-stu-id="9bc29-113">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="9bc29-114">Abrufen von privilegedRole</span><span class="sxs-lookup"><span data-stu-id="9bc29-114">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="9bc29-115">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="9bc29-115">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="9bc29-116">Lesen Sie Eigenschaften und Beziehungen des PrivilegedRole-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9bc29-116">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="9bc29-117">Liste Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="9bc29-117">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="9bc29-118">[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9bc29-118">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="9bc29-119">Rufen Sie eine Assignment-Objekt-Auflistung für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="9bc29-119">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="9bc29-120">selfActivate</span><span class="sxs-lookup"><span data-stu-id="9bc29-120">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="9bc29-121">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9bc29-121">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="9bc29-122">Aktivieren Sie die zugeordnete Rolle.</span><span class="sxs-lookup"><span data-stu-id="9bc29-122">Activate the assigned role.</span></span>|
|[<span data-ttu-id="9bc29-123">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="9bc29-123">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="9bc29-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9bc29-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="9bc29-125">Deaktivieren Sie die zugeordnete Rolle.</span><span class="sxs-lookup"><span data-stu-id="9bc29-125">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="9bc29-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9bc29-126">Properties</span></span>
| <span data-ttu-id="9bc29-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9bc29-127">Property</span></span>     | <span data-ttu-id="9bc29-128">Typ</span><span class="sxs-lookup"><span data-stu-id="9bc29-128">Type</span></span>   |<span data-ttu-id="9bc29-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bc29-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bc29-130">id</span><span class="sxs-lookup"><span data-stu-id="9bc29-130">id</span></span>|<span data-ttu-id="9bc29-131">string</span><span class="sxs-lookup"><span data-stu-id="9bc29-131">string</span></span>|<span data-ttu-id="9bc29-132">Der eindeutige Bezeichner für Administratorrolle.</span><span class="sxs-lookup"><span data-stu-id="9bc29-132">The unique identifier for administrator role.</span></span> <span data-ttu-id="9bc29-133">Es ist eine GUID-Zeichenfolge und hat den gleichen Wert wie der Rolle Vorlagen-Id aus dem Azure Active Directory für die gegebene Rolle.</span><span class="sxs-lookup"><span data-stu-id="9bc29-133">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="9bc29-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9bc29-134">Read-only.</span></span>|
|<span data-ttu-id="9bc29-135">name</span><span class="sxs-lookup"><span data-stu-id="9bc29-135">name</span></span>|<span data-ttu-id="9bc29-136">string</span><span class="sxs-lookup"><span data-stu-id="9bc29-136">string</span></span>|<span data-ttu-id="9bc29-137">Rollenname.</span><span class="sxs-lookup"><span data-stu-id="9bc29-137">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bc29-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9bc29-138">Relationships</span></span>
| <span data-ttu-id="9bc29-139">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9bc29-139">Relationship</span></span> | <span data-ttu-id="9bc29-140">Typ</span><span class="sxs-lookup"><span data-stu-id="9bc29-140">Type</span></span>   |<span data-ttu-id="9bc29-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bc29-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bc29-142">assignments</span><span class="sxs-lookup"><span data-stu-id="9bc29-142">assignments</span></span>|<span data-ttu-id="9bc29-143">[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9bc29-143">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="9bc29-144">Die Zuordnungen für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="9bc29-144">The assignments for this role.</span></span> <span data-ttu-id="9bc29-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9bc29-145">Read-only.</span></span> <span data-ttu-id="9bc29-146">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="9bc29-146">Nullable.</span></span>|
|<span data-ttu-id="9bc29-147">settings</span><span class="sxs-lookup"><span data-stu-id="9bc29-147">settings</span></span>|[<span data-ttu-id="9bc29-148">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9bc29-148">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="9bc29-149">Die Einstellungen für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="9bc29-149">The settings for this role.</span></span> <span data-ttu-id="9bc29-150">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9bc29-150">Read-only.</span></span> <span data-ttu-id="9bc29-151">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="9bc29-151">Nullable.</span></span>|
|<span data-ttu-id="9bc29-152">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="9bc29-152">summary</span></span>|[<span data-ttu-id="9bc29-153">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="9bc29-153">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="9bc29-154">Der zusammenfassende Informationen für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="9bc29-154">The summary information for this role.</span></span> <span data-ttu-id="9bc29-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9bc29-155">Read-only.</span></span> <span data-ttu-id="9bc29-156">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="9bc29-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9bc29-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9bc29-157">JSON representation</span></span>

<span data-ttu-id="9bc29-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9bc29-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRole"
}-->

```json
{
  "id": "string (identifier)",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->