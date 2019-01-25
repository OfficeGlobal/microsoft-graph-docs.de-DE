---
title: Ressourcentyp privilegedRoleAssignment
description: 'Stellt eine privilegierten rollenzuweisung für einen bestimmten Benutzer. '
localization_priority: Normal
ms.openlocfilehash: 479b6d46dc479134fd0abb46b1a9ffe478611a82
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515118"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="ef024-103">Ressourcentyp privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ef024-103">privilegedRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef024-104">Stellt eine privilegierten rollenzuweisung für einen bestimmten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="ef024-104">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="ef024-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="ef024-105">Methods</span></span>

| <span data-ttu-id="ef024-106">Methode</span><span class="sxs-lookup"><span data-stu-id="ef024-106">Method</span></span>           | <span data-ttu-id="ef024-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ef024-107">Return Type</span></span>    |<span data-ttu-id="ef024-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef024-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef024-109">Liste PrivilegedRoleAssignment-Auflistung</span><span class="sxs-lookup"><span data-stu-id="ef024-109">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="ef024-110">[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ef024-110">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="ef024-111">Rufen Sie die Auflistung von PrivilegedRoleAssignment-Objekten.</span><span class="sxs-lookup"><span data-stu-id="ef024-111">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="ef024-112">Abrufen von privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ef024-112">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="ef024-113">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ef024-113">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="ef024-114">Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleAssignment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ef024-114">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="ef024-115">Erstellen der Zuordnung</span><span class="sxs-lookup"><span data-stu-id="ef024-115">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="ef024-116">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ef024-116">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="ef024-117">Erstellen Sie eine neue Zuordnung, indem Sie das Veröffentlichen in der Assignments-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="ef024-117">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="ef024-118">Delete</span><span class="sxs-lookup"><span data-stu-id="ef024-118">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="ef024-119">Keine</span><span class="sxs-lookup"><span data-stu-id="ef024-119">None</span></span> |<span data-ttu-id="ef024-120">PrivilegedRoleAssignment-Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="ef024-120">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="ef024-121">makePermanent</span><span class="sxs-lookup"><span data-stu-id="ef024-121">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="ef024-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ef024-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="ef024-123">Stellen Sie die rollenzuweisung als dauerhaft entfernt.</span><span class="sxs-lookup"><span data-stu-id="ef024-123">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="ef024-124">makeEligible</span><span class="sxs-lookup"><span data-stu-id="ef024-124">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="ef024-125">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ef024-125">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="ef024-126">Stellen Sie die rollenzuweisung als geeignet.</span><span class="sxs-lookup"><span data-stu-id="ef024-126">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="ef024-127">My</span><span class="sxs-lookup"><span data-stu-id="ef024-127">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="ef024-128">[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ef024-128">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="ef024-129">Abrufen des aktuellen Benutzers privilegierten rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="ef024-129">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="ef024-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ef024-130">Properties</span></span>
| <span data-ttu-id="ef024-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ef024-131">Property</span></span>     | <span data-ttu-id="ef024-132">Typ</span><span class="sxs-lookup"><span data-stu-id="ef024-132">Type</span></span>   |<span data-ttu-id="ef024-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef024-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef024-134">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ef024-134">expirationDateTime</span></span>|<span data-ttu-id="ef024-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef024-135">dateTimeOffset</span></span>|<span data-ttu-id="ef024-136">Die UTC-DateTime, die temporäre privilegierten rollenzuweisung abgelaufen sein wird.</span><span class="sxs-lookup"><span data-stu-id="ef024-136">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="ef024-137">Für permanente rollenzuweisung ist der Wert null.</span><span class="sxs-lookup"><span data-stu-id="ef024-137">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="ef024-138">id</span><span class="sxs-lookup"><span data-stu-id="ef024-138">id</span></span>|<span data-ttu-id="ef024-139">string</span><span class="sxs-lookup"><span data-stu-id="ef024-139">string</span></span>| <span data-ttu-id="ef024-140">Der eindeutige Bezeichner für die privilegierten rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="ef024-140">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="ef024-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ef024-141">Read-only.</span></span> <span data-ttu-id="ef024-142">Es ist im Format "UserId_roleId", wobei Benutzer-ID ist die GUID-Zeichenfolge für Azure AD-Benutzer-Id und RoleId ist die GUID für Azure Administrator Rollen-Id-Zeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="ef024-142">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="ef024-143">isElevated</span><span class="sxs-lookup"><span data-stu-id="ef024-143">isElevated</span></span>|<span data-ttu-id="ef024-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ef024-144">boolean</span></span>|<span data-ttu-id="ef024-145">**true,** Wenn die rollenzuweisung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="ef024-145">**true** if the role assignment is activated.</span></span> <span data-ttu-id="ef024-146">**false,** Wenn die rollenzuweisung deaktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="ef024-146">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="ef024-147">resultMessage</span><span class="sxs-lookup"><span data-stu-id="ef024-147">resultMessage</span></span>|<span data-ttu-id="ef024-148">string</span><span class="sxs-lookup"><span data-stu-id="ef024-148">string</span></span>|<span data-ttu-id="ef024-149">Ergebnisnachricht vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ef024-149">Result message set by the service.</span></span>|
|<span data-ttu-id="ef024-150">roleId</span><span class="sxs-lookup"><span data-stu-id="ef024-150">roleId</span></span>|<span data-ttu-id="ef024-151">string</span><span class="sxs-lookup"><span data-stu-id="ef024-151">string</span></span>|<span data-ttu-id="ef024-152">Rollenbezeichner</span><span class="sxs-lookup"><span data-stu-id="ef024-152">Role identifier.</span></span> <span data-ttu-id="ef024-153">Im Zeichenformat GUID.</span><span class="sxs-lookup"><span data-stu-id="ef024-153">In GUID string format.</span></span>|
|<span data-ttu-id="ef024-154">userId</span><span class="sxs-lookup"><span data-stu-id="ef024-154">userId</span></span>|<span data-ttu-id="ef024-155">string</span><span class="sxs-lookup"><span data-stu-id="ef024-155">string</span></span>|<span data-ttu-id="ef024-156">Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="ef024-156">User identifier.</span></span> <span data-ttu-id="ef024-157">Im Zeichenformat GUID.</span><span class="sxs-lookup"><span data-stu-id="ef024-157">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef024-158">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ef024-158">Relationships</span></span>
| <span data-ttu-id="ef024-159">Beziehung</span><span class="sxs-lookup"><span data-stu-id="ef024-159">Relationship</span></span> | <span data-ttu-id="ef024-160">Typ</span><span class="sxs-lookup"><span data-stu-id="ef024-160">Type</span></span>   |<span data-ttu-id="ef024-161">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef024-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef024-162">roleInfo</span><span class="sxs-lookup"><span data-stu-id="ef024-162">roleInfo</span></span>|[<span data-ttu-id="ef024-163">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="ef024-163">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="ef024-164">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ef024-164">Read-only.</span></span> <span data-ttu-id="ef024-165">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="ef024-165">Nullable.</span></span> <span data-ttu-id="ef024-166">Die zugehörige Rolle-Informationen.</span><span class="sxs-lookup"><span data-stu-id="ef024-166">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef024-167">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ef024-167">JSON representation</span></span>

<span data-ttu-id="ef024-168">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ef024-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
