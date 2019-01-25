---
title: Ressourcentyp privilegedRole
description: 'Stellt eine Azure AD-Administratorrolle z. B.: **globaler Administrator, Abrechnungsadministrator, Dienstadministrator, Benutzer-Administrator, Kennwort-Administrator**usw..'
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513746"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="d93da-103">Ressourcentyp privilegedRole</span><span class="sxs-lookup"><span data-stu-id="d93da-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d93da-104">Stellt eine Azure AD-Administratorrolle z. B.: **globaler Administrator, Abrechnungsadministrator, Dienstadministrator, Benutzer-Administrator, Kennwort-Administrator**usw..</span><span class="sxs-lookup"><span data-stu-id="d93da-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="d93da-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d93da-105">Methods</span></span>

| <span data-ttu-id="d93da-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d93da-106">Method</span></span>           | <span data-ttu-id="d93da-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d93da-107">Return Type</span></span>    |<span data-ttu-id="d93da-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d93da-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d93da-109">Objekte in der Liste privilegedRole</span><span class="sxs-lookup"><span data-stu-id="d93da-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="d93da-110">[PrivilegedRole](privilegedrole.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d93da-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="d93da-111">Ruft die Auflistung der PrivilegedRole.</span><span class="sxs-lookup"><span data-stu-id="d93da-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="d93da-112">Abrufen von privilegedRole</span><span class="sxs-lookup"><span data-stu-id="d93da-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="d93da-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="d93da-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="d93da-114">Lesen Sie Eigenschaften und Beziehungen des PrivilegedRole-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d93da-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="d93da-115">Liste Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="d93da-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="d93da-116">[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d93da-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="d93da-117">Rufen Sie eine Assignment-Objekt-Auflistung für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="d93da-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="d93da-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="d93da-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="d93da-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d93da-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="d93da-120">Aktivieren Sie die zugeordnete Rolle.</span><span class="sxs-lookup"><span data-stu-id="d93da-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="d93da-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="d93da-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="d93da-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d93da-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="d93da-123">Deaktivieren Sie die zugeordnete Rolle.</span><span class="sxs-lookup"><span data-stu-id="d93da-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="d93da-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d93da-124">Properties</span></span>
| <span data-ttu-id="d93da-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d93da-125">Property</span></span>     | <span data-ttu-id="d93da-126">Typ</span><span class="sxs-lookup"><span data-stu-id="d93da-126">Type</span></span>   |<span data-ttu-id="d93da-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d93da-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d93da-128">id</span><span class="sxs-lookup"><span data-stu-id="d93da-128">id</span></span>|<span data-ttu-id="d93da-129">string</span><span class="sxs-lookup"><span data-stu-id="d93da-129">string</span></span>|<span data-ttu-id="d93da-130">Der eindeutige Bezeichner für Administratorrolle.</span><span class="sxs-lookup"><span data-stu-id="d93da-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="d93da-131">Es ist eine GUID-Zeichenfolge und hat den gleichen Wert wie der Rolle Vorlagen-Id aus dem Azure Active Directory für die gegebene Rolle.</span><span class="sxs-lookup"><span data-stu-id="d93da-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="d93da-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d93da-132">Read-only.</span></span>|
|<span data-ttu-id="d93da-133">name</span><span class="sxs-lookup"><span data-stu-id="d93da-133">name</span></span>|<span data-ttu-id="d93da-134">string</span><span class="sxs-lookup"><span data-stu-id="d93da-134">string</span></span>|<span data-ttu-id="d93da-135">Rollenname.</span><span class="sxs-lookup"><span data-stu-id="d93da-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d93da-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d93da-136">Relationships</span></span>
| <span data-ttu-id="d93da-137">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d93da-137">Relationship</span></span> | <span data-ttu-id="d93da-138">Typ</span><span class="sxs-lookup"><span data-stu-id="d93da-138">Type</span></span>   |<span data-ttu-id="d93da-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d93da-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d93da-140">assignments</span><span class="sxs-lookup"><span data-stu-id="d93da-140">assignments</span></span>|<span data-ttu-id="d93da-141">[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d93da-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="d93da-142">Die Zuordnungen für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="d93da-142">The assignments for this role.</span></span> <span data-ttu-id="d93da-143">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d93da-143">Read-only.</span></span> <span data-ttu-id="d93da-144">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="d93da-144">Nullable.</span></span>|
|<span data-ttu-id="d93da-145">settings</span><span class="sxs-lookup"><span data-stu-id="d93da-145">settings</span></span>|[<span data-ttu-id="d93da-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="d93da-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="d93da-147">Die Einstellungen für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="d93da-147">The settings for this role.</span></span> <span data-ttu-id="d93da-148">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d93da-148">Read-only.</span></span> <span data-ttu-id="d93da-149">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="d93da-149">Nullable.</span></span>|
|<span data-ttu-id="d93da-150">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="d93da-150">summary</span></span>|[<span data-ttu-id="d93da-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="d93da-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="d93da-152">Der zusammenfassende Informationen für diese Rolle.</span><span class="sxs-lookup"><span data-stu-id="d93da-152">The summary information for this role.</span></span> <span data-ttu-id="d93da-153">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d93da-153">Read-only.</span></span> <span data-ttu-id="d93da-154">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="d93da-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d93da-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d93da-155">JSON representation</span></span>

<span data-ttu-id="d93da-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d93da-156">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
