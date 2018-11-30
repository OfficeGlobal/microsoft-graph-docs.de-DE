---
title: Ressourcentyp privilegedRoleAssignment
description: 'Stellt eine privilegierten rollenzuweisung für einen bestimmten Benutzer. '
ms.openlocfilehash: 40cfe6487184171fc0d120f9a0e2cd98070f96f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060252"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="66572-103">Ressourcentyp privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="66572-103">privilegedRoleAssignment resource type</span></span>

> <span data-ttu-id="66572-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="66572-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66572-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66572-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66572-106">Stellt eine privilegierten rollenzuweisung für einen bestimmten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="66572-106">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="66572-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="66572-107">Methods</span></span>

| <span data-ttu-id="66572-108">Methode</span><span class="sxs-lookup"><span data-stu-id="66572-108">Method</span></span>           | <span data-ttu-id="66572-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="66572-109">Return Type</span></span>    |<span data-ttu-id="66572-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66572-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="66572-111">Liste PrivilegedRoleAssignment-Auflistung</span><span class="sxs-lookup"><span data-stu-id="66572-111">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="66572-112">[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="66572-112">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="66572-113">Rufen Sie die Auflistung von PrivilegedRoleAssignment-Objekten.</span><span class="sxs-lookup"><span data-stu-id="66572-113">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="66572-114">Abrufen von privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="66572-114">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="66572-115">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="66572-115">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="66572-116">Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleAssignment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="66572-116">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="66572-117">Erstellen der Zuordnung</span><span class="sxs-lookup"><span data-stu-id="66572-117">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="66572-118">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="66572-118">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="66572-119">Erstellen Sie eine neue Zuordnung, indem Sie das Veröffentlichen in der Assignments-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="66572-119">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="66572-120">Delete</span><span class="sxs-lookup"><span data-stu-id="66572-120">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="66572-121">Keine</span><span class="sxs-lookup"><span data-stu-id="66572-121">None</span></span> |<span data-ttu-id="66572-122">PrivilegedRoleAssignment-Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="66572-122">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="66572-123">makePermanent</span><span class="sxs-lookup"><span data-stu-id="66572-123">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="66572-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="66572-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="66572-125">Stellen Sie die rollenzuweisung als dauerhaft entfernt.</span><span class="sxs-lookup"><span data-stu-id="66572-125">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="66572-126">makeEligible</span><span class="sxs-lookup"><span data-stu-id="66572-126">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="66572-127">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="66572-127">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="66572-128">Stellen Sie die rollenzuweisung als geeignet.</span><span class="sxs-lookup"><span data-stu-id="66572-128">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="66572-129">Meine</span><span class="sxs-lookup"><span data-stu-id="66572-129">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="66572-130">[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="66572-130">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="66572-131">Abrufen des aktuellen Benutzers privilegierten rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="66572-131">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="66572-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66572-132">Properties</span></span>
| <span data-ttu-id="66572-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66572-133">Property</span></span>     | <span data-ttu-id="66572-134">Typ</span><span class="sxs-lookup"><span data-stu-id="66572-134">Type</span></span>   |<span data-ttu-id="66572-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66572-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66572-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="66572-136">expirationDateTime</span></span>|<span data-ttu-id="66572-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66572-137">dateTimeOffset</span></span>|<span data-ttu-id="66572-138">Die UTC-DateTime, die temporäre privilegierten rollenzuweisung abgelaufen sein wird.</span><span class="sxs-lookup"><span data-stu-id="66572-138">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="66572-139">Für permanente rollenzuweisung ist der Wert null.</span><span class="sxs-lookup"><span data-stu-id="66572-139">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="66572-140">id</span><span class="sxs-lookup"><span data-stu-id="66572-140">id</span></span>|<span data-ttu-id="66572-141">string</span><span class="sxs-lookup"><span data-stu-id="66572-141">string</span></span>| <span data-ttu-id="66572-142">Der eindeutige Bezeichner für die privilegierten rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="66572-142">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="66572-143">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="66572-143">Read-only.</span></span> <span data-ttu-id="66572-144">Es ist im Format "UserId_roleId", wobei Benutzer-ID ist die GUID-Zeichenfolge für Azure AD-Benutzer-Id und RoleId ist die GUID für Azure Administrator Rollen-Id-Zeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="66572-144">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="66572-145">isElevated</span><span class="sxs-lookup"><span data-stu-id="66572-145">isElevated</span></span>|<span data-ttu-id="66572-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="66572-146">boolean</span></span>|<span data-ttu-id="66572-147">**true,** Wenn die rollenzuweisung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="66572-147">**true** if the role assignment is activated.</span></span> <span data-ttu-id="66572-148">**false,** Wenn die rollenzuweisung deaktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="66572-148">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="66572-149">resultMessage</span><span class="sxs-lookup"><span data-stu-id="66572-149">resultMessage</span></span>|<span data-ttu-id="66572-150">string</span><span class="sxs-lookup"><span data-stu-id="66572-150">string</span></span>|<span data-ttu-id="66572-151">Ergebnisnachricht vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="66572-151">Result message set by the service.</span></span>|
|<span data-ttu-id="66572-152">roleId</span><span class="sxs-lookup"><span data-stu-id="66572-152">roleId</span></span>|<span data-ttu-id="66572-153">string</span><span class="sxs-lookup"><span data-stu-id="66572-153">string</span></span>|<span data-ttu-id="66572-154">Rollenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="66572-154">Role identifier.</span></span> <span data-ttu-id="66572-155">Im Zeichenformat GUID.</span><span class="sxs-lookup"><span data-stu-id="66572-155">In GUID string format.</span></span>|
|<span data-ttu-id="66572-156">userId</span><span class="sxs-lookup"><span data-stu-id="66572-156">userId</span></span>|<span data-ttu-id="66572-157">string</span><span class="sxs-lookup"><span data-stu-id="66572-157">string</span></span>|<span data-ttu-id="66572-158">Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="66572-158">User identifier.</span></span> <span data-ttu-id="66572-159">Im Zeichenformat GUID.</span><span class="sxs-lookup"><span data-stu-id="66572-159">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66572-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="66572-160">Relationships</span></span>
| <span data-ttu-id="66572-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="66572-161">Relationship</span></span> | <span data-ttu-id="66572-162">Typ</span><span class="sxs-lookup"><span data-stu-id="66572-162">Type</span></span>   |<span data-ttu-id="66572-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66572-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66572-164">roleInfo</span><span class="sxs-lookup"><span data-stu-id="66572-164">roleInfo</span></span>|[<span data-ttu-id="66572-165">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="66572-165">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="66572-166">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="66572-166">Read-only.</span></span> <span data-ttu-id="66572-167">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="66572-167">Nullable.</span></span> <span data-ttu-id="66572-168">Die zugehörige Rolle-Informationen.</span><span class="sxs-lookup"><span data-stu-id="66572-168">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66572-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66572-169">JSON representation</span></span>

<span data-ttu-id="66572-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="66572-170">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->