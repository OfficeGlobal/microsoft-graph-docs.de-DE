---
title: appRoleAssignment-Ressourcentyp
description: Dient zum Aufzeichnen, wann ein Benutzer oder eine Gruppe einer Anwendung zugewiesen wird. In diesem Fall führt die Rollenzuweisung dazu, dass die Anwendungskachel im App-Zugriffsbereich des Benutzers angezeigt wird. Diese Entität kann auch verwendet werden, um einer anderen Anwendung (als Dienstprinzipal modelliert) Zugriff auf eine Ressourcenanwendung in einer bestimmten Rolle zu gewähren. Sie können Rollenzuweisungen erstellen, lesen, aktualisieren und löschen.
localization_priority: Priority
ms.openlocfilehash: 6255642f47f0e1454fb64440d4938605a2de5df4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513900"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="03568-106">appRoleAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="03568-106">appRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03568-107">Dient zum Aufzeichnen, wann ein Benutzer oder eine Gruppe einer Anwendung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="03568-107">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="03568-108">In diesem Fall führt die Rollenzuweisung dazu, dass die Anwendungskachel im App-Zugriffsbereich des Benutzers angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="03568-108">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="03568-109">Diese Entität kann auch verwendet werden, um einer anderen Anwendung (als Dienstprinzipal modelliert) Zugriff auf eine Ressourcenanwendung in einer bestimmten Rolle zu gewähren.</span><span class="sxs-lookup"><span data-stu-id="03568-109">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="03568-110">Sie können Rollenzuweisungen erstellen, lesen, aktualisieren und löschen.</span><span class="sxs-lookup"><span data-stu-id="03568-110">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="03568-111">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="03568-111">JSON representation</span></span>

<span data-ttu-id="03568-112">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="03568-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approleassignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a><span data-ttu-id="03568-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="03568-113">Properties</span></span>
| <span data-ttu-id="03568-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03568-114">Property</span></span>     | <span data-ttu-id="03568-115">Typ</span><span class="sxs-lookup"><span data-stu-id="03568-115">Type</span></span>   |<span data-ttu-id="03568-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03568-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03568-117">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="03568-117">creationTimestamp</span></span>|<span data-ttu-id="03568-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03568-118">DateTimeOffset</span></span>|<span data-ttu-id="03568-119">Der Zeitpunkt, zu dem der Kontakt erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: </span><span class="sxs-lookup"><span data-stu-id="03568-119">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="03568-120">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="03568-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="03568-121">id</span><span class="sxs-lookup"><span data-stu-id="03568-121">id</span></span>|<span data-ttu-id="03568-122">Guid</span><span class="sxs-lookup"><span data-stu-id="03568-122">Guid</span></span>|<span data-ttu-id="03568-123">Die Rollen-ID, die dem Prinzipal zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="03568-123">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="03568-124">Diese Rolle muss von der Zielressourcenanwendung **ResourceId** in der **appRoles**-Eigenschaft deklariert werden.</span><span class="sxs-lookup"><span data-stu-id="03568-124">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="03568-125">Wenn die Ressource keine Berechtigungen deklariert, muss eine Standard-ID (GUID von 0) angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="03568-125">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="03568-126">Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="03568-126">Key.</span></span> <span data-ttu-id="03568-127">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="03568-127">Not nullable.</span></span> |
|<span data-ttu-id="03568-128">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="03568-128">principalDisplayName</span></span>|<span data-ttu-id="03568-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="03568-129">String</span></span>|<span data-ttu-id="03568-130">Der Anzeigename des Prinzipals, dem Zugriff gewährt wurde.</span><span class="sxs-lookup"><span data-stu-id="03568-130">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="03568-131">principalId</span><span class="sxs-lookup"><span data-stu-id="03568-131">principalId</span></span>|<span data-ttu-id="03568-132">Guid</span><span class="sxs-lookup"><span data-stu-id="03568-132">Guid</span></span>|<span data-ttu-id="03568-133">Der eindeutige Bezeichner (**Id**) für den Prinzipal, dem Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="03568-133">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="03568-134">Beim Erstellen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="03568-134">Required on create.</span></span>            |
|<span data-ttu-id="03568-135">principalType</span><span class="sxs-lookup"><span data-stu-id="03568-135">principalType</span></span>|<span data-ttu-id="03568-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="03568-136">String</span></span>|<span data-ttu-id="03568-137">Der Prinzipaltyp.</span><span class="sxs-lookup"><span data-stu-id="03568-137">The type of principal.</span></span>  <span data-ttu-id="03568-138">Dies kann entweder „Benutzer“, „Gruppe“ oder „ServicePrincipal“ sein.</span><span class="sxs-lookup"><span data-stu-id="03568-138">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="03568-139">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="03568-139">resourceDisplayName</span></span>|<span data-ttu-id="03568-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="03568-140">String</span></span>|<span data-ttu-id="03568-141">Der Anzeigename der Ressource, für die die Zuweisung erfolgte.</span><span class="sxs-lookup"><span data-stu-id="03568-141">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="03568-142">resourceId</span><span class="sxs-lookup"><span data-stu-id="03568-142">resourceId</span></span>|<span data-ttu-id="03568-143">Guid</span><span class="sxs-lookup"><span data-stu-id="03568-143">Guid</span></span>|<span data-ttu-id="03568-144">Die eindeutige ID (**Id**) für die Zielressource (Dienstprinzipal), für die die Zuweisung vorgenommen wurde.</span><span class="sxs-lookup"><span data-stu-id="03568-144">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03568-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="03568-145">Relationships</span></span>
<span data-ttu-id="03568-146">Keine</span><span class="sxs-lookup"><span data-stu-id="03568-146">None</span></span>


## <a name="methods"></a><span data-ttu-id="03568-147">Methoden</span><span class="sxs-lookup"><span data-stu-id="03568-147">Methods</span></span>

| <span data-ttu-id="03568-148">Methode</span><span class="sxs-lookup"><span data-stu-id="03568-148">Method</span></span>           | <span data-ttu-id="03568-149">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="03568-149">Return Type</span></span>    |<span data-ttu-id="03568-150">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03568-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03568-151">appRoleAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="03568-151">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="03568-152">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="03568-152">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="03568-153">Lesen von Eigenschaften und Beziehungen des approleAssignment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="03568-153">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="03568-154">Update</span><span class="sxs-lookup"><span data-stu-id="03568-154">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="03568-155">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="03568-155">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="03568-156">Aktualisieren des approleassignment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="03568-156">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="03568-157">Delete</span><span class="sxs-lookup"><span data-stu-id="03568-157">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="03568-158">Keine</span><span class="sxs-lookup"><span data-stu-id="03568-158">None</span></span> |<span data-ttu-id="03568-159">Löschen des approleassignment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="03568-159">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
