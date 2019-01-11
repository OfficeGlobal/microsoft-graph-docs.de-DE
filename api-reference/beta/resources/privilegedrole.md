---
title: Ressourcentyp privilegedRole
description: 'Stellt eine Azure AD-Administratorrolle z. B.: **globaler Administrator, Abrechnungsadministrator, Dienstadministrator, Benutzer-Administrator, Kennwort-Administrator**usw..'
localization_priority: Normal
ms.openlocfilehash: 75763e18731cb969623cc4df6360d50abc018b41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860858"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="44176-103">Ressourcentyp privilegedRole</span><span class="sxs-lookup"><span data-stu-id="44176-103">privilegedRole resource type</span></span>

> <span data-ttu-id="44176-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="44176-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44176-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44176-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44176-106">Stellt eine Azure AD-Administratorrolle z. B.: **globaler Administrator, Abrechnungsadministrator, Dienstadministrator, Benutzer-Administrator, Kennwort-Administrator**usw..</span><span class="sxs-lookup"><span data-stu-id="44176-106">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="44176-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="44176-107">Methods</span></span>

| <span data-ttu-id="44176-108">Methode</span><span class="sxs-lookup"><span data-stu-id="44176-108">Method</span></span>           | <span data-ttu-id="44176-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="44176-109">Return Type</span></span>    |<span data-ttu-id="44176-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44176-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="44176-111">Objekte in der Liste privilegedRole</span><span class="sxs-lookup"><span data-stu-id="44176-111">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="44176-112">[PrivilegedRole](privilegedrole.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="44176-112">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="44176-113">Ruft die Auflistung der PrivilegedRole.</span><span class="sxs-lookup"><span data-stu-id="44176-113">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="44176-114">Abrufen von privilegedRole</span><span class="sxs-lookup"><span data-stu-id="44176-114">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="44176-115">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="44176-115">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="44176-116">Lesen Sie Eigenschaften und Beziehungen des PrivilegedRole-Objekts.</span><span class="sxs-lookup"><span data-stu-id="44176-116">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="44176-117">Liste Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="44176-117">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="44176-118">[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="44176-118">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="44176-119">Rufen Sie eine Assignment-Objekt-Auflistung für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="44176-119">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="44176-120">selfActivate</span><span class="sxs-lookup"><span data-stu-id="44176-120">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="44176-121">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="44176-121">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="44176-122">Aktivieren Sie die zugeordnete Rolle.</span><span class="sxs-lookup"><span data-stu-id="44176-122">Activate the assigned role.</span></span>|
|[<span data-ttu-id="44176-123">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="44176-123">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="44176-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="44176-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="44176-125">Deaktivieren Sie die zugeordnete Rolle.</span><span class="sxs-lookup"><span data-stu-id="44176-125">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="44176-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="44176-126">Properties</span></span>
| <span data-ttu-id="44176-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="44176-127">Property</span></span>     | <span data-ttu-id="44176-128">Typ</span><span class="sxs-lookup"><span data-stu-id="44176-128">Type</span></span>   |<span data-ttu-id="44176-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44176-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44176-130">id</span><span class="sxs-lookup"><span data-stu-id="44176-130">id</span></span>|<span data-ttu-id="44176-131">string</span><span class="sxs-lookup"><span data-stu-id="44176-131">string</span></span>|<span data-ttu-id="44176-132">Der eindeutige Bezeichner für Administratorrolle.</span><span class="sxs-lookup"><span data-stu-id="44176-132">The unique identifier for administrator role.</span></span> <span data-ttu-id="44176-133">Es ist eine GUID-Zeichenfolge und hat den gleichen Wert wie der Rolle Vorlagen-Id aus dem Azure Active Directory für die gegebene Rolle.</span><span class="sxs-lookup"><span data-stu-id="44176-133">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="44176-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="44176-134">Read-only.</span></span>|
|<span data-ttu-id="44176-135">name</span><span class="sxs-lookup"><span data-stu-id="44176-135">name</span></span>|<span data-ttu-id="44176-136">string</span><span class="sxs-lookup"><span data-stu-id="44176-136">string</span></span>|<span data-ttu-id="44176-137">Rollenname.</span><span class="sxs-lookup"><span data-stu-id="44176-137">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44176-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="44176-138">Relationships</span></span>
| <span data-ttu-id="44176-139">Beziehung</span><span class="sxs-lookup"><span data-stu-id="44176-139">Relationship</span></span> | <span data-ttu-id="44176-140">Typ</span><span class="sxs-lookup"><span data-stu-id="44176-140">Type</span></span>   |<span data-ttu-id="44176-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44176-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44176-142">assignments</span><span class="sxs-lookup"><span data-stu-id="44176-142">assignments</span></span>|<span data-ttu-id="44176-143">[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="44176-143">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="44176-144">Die Zuordnungen für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="44176-144">The assignments for this role.</span></span> <span data-ttu-id="44176-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="44176-145">Read-only.</span></span> <span data-ttu-id="44176-146">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="44176-146">Nullable.</span></span>|
|<span data-ttu-id="44176-147">settings</span><span class="sxs-lookup"><span data-stu-id="44176-147">settings</span></span>|[<span data-ttu-id="44176-148">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="44176-148">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="44176-149">Die Einstellungen für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="44176-149">The settings for this role.</span></span> <span data-ttu-id="44176-150">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="44176-150">Read-only.</span></span> <span data-ttu-id="44176-151">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="44176-151">Nullable.</span></span>|
|<span data-ttu-id="44176-152">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="44176-152">summary</span></span>|[<span data-ttu-id="44176-153">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="44176-153">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="44176-154">Der zusammenfassende Informationen für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="44176-154">The summary information for this role.</span></span> <span data-ttu-id="44176-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="44176-155">Read-only.</span></span> <span data-ttu-id="44176-156">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="44176-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44176-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="44176-157">JSON representation</span></span>

<span data-ttu-id="44176-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="44176-158">Here is a JSON representation of the resource.</span></span>

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
