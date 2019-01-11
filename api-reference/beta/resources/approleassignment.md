---
title: Ressourcentyp appRoleAssignment
description: Verwendet zum Aufzeichnen, wenn ein Benutzer oder eine Gruppe zu einer Anwendung zugewiesen wird. In diesem Fall führt die rollenzuweisung Kachel Anwendung Einrichten des Benutzers app Zugriff im Bereich angezeigt. Dieser Entität kann auch verwendet werden, zu einer anderen (modelliert als Dienst principal) Anwendungszugriff auf eine Ressource-Anwendung in einer bestimmten Rolle erteilen. Sie können erstellen, lesen, aktualisieren und Löschen von rollenzuweisungen.
localization_priority: Priority
ms.openlocfilehash: 3276c1f34b91dc628ed00f2ffbc64ffe56899bdf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845472"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="e68aa-106">Ressourcentyp appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e68aa-106">appRoleAssignment resource type</span></span>

> <span data-ttu-id="e68aa-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e68aa-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e68aa-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e68aa-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e68aa-109">Verwendet zum Aufzeichnen, wenn ein Benutzer oder eine Gruppe zu einer Anwendung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="e68aa-109">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="e68aa-110">In diesem Fall führt die rollenzuweisung Kachel Anwendung Einrichten des Benutzers app Zugriff im Bereich angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e68aa-110">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="e68aa-111">Dieser Entität kann auch verwendet werden, zu einer anderen (modelliert als Dienst principal) Anwendungszugriff auf eine Ressource-Anwendung in einer bestimmten Rolle erteilen.</span><span class="sxs-lookup"><span data-stu-id="e68aa-111">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="e68aa-112">Sie können erstellen, lesen, aktualisieren und Löschen von rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="e68aa-112">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e68aa-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e68aa-113">JSON representation</span></span>

<span data-ttu-id="e68aa-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e68aa-114">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="e68aa-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e68aa-115">Properties</span></span>
| <span data-ttu-id="e68aa-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e68aa-116">Property</span></span>     | <span data-ttu-id="e68aa-117">Typ</span><span class="sxs-lookup"><span data-stu-id="e68aa-117">Type</span></span>   |<span data-ttu-id="e68aa-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e68aa-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e68aa-119">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="e68aa-119">creationTimestamp</span></span>|<span data-ttu-id="e68aa-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e68aa-120">DateTimeOffset</span></span>|<span data-ttu-id="e68aa-121">Die Uhrzeit der Erstellung der erteilen. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="e68aa-121">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e68aa-122">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e68aa-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e68aa-123">id</span><span class="sxs-lookup"><span data-stu-id="e68aa-123">id</span></span>|<span data-ttu-id="e68aa-124">Guid</span><span class="sxs-lookup"><span data-stu-id="e68aa-124">Guid</span></span>|<span data-ttu-id="e68aa-125">Die Rolle-Id, die den Prinzipal zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="e68aa-125">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="e68aa-126">Diese Rolle muss mit der Ziel-Ressource Anwendung **ResourceId** in seiner **AppRoles** -Eigenschaft deklariert werden.</span><span class="sxs-lookup"><span data-stu-id="e68aa-126">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="e68aa-127">In denen die Ressource keine Berechtigungen nicht deklarieren, muss eine Standard-Id (0 (null) GUID) angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e68aa-127">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="e68aa-128">Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="e68aa-128">Key.</span></span> <span data-ttu-id="e68aa-129">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="e68aa-129">Not nullable.</span></span> |
|<span data-ttu-id="e68aa-130">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="e68aa-130">principalDisplayName</span></span>|<span data-ttu-id="e68aa-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e68aa-131">String</span></span>|<span data-ttu-id="e68aa-132">Der Anzeigename des Prinzipals, die der Zugriff gewährt wurde.</span><span class="sxs-lookup"><span data-stu-id="e68aa-132">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="e68aa-133">principalId</span><span class="sxs-lookup"><span data-stu-id="e68aa-133">principalId</span></span>|<span data-ttu-id="e68aa-134">Guid</span><span class="sxs-lookup"><span data-stu-id="e68aa-134">Guid</span></span>|<span data-ttu-id="e68aa-135">Der eindeutige Bezeichner (**Id**) für den Prinzipal, den Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="e68aa-135">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="e68aa-136">Erforderliche auf erstellen.</span><span class="sxs-lookup"><span data-stu-id="e68aa-136">Required on create.</span></span>            |
|<span data-ttu-id="e68aa-137">principalType</span><span class="sxs-lookup"><span data-stu-id="e68aa-137">principalType</span></span>|<span data-ttu-id="e68aa-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e68aa-138">String</span></span>|<span data-ttu-id="e68aa-139">Der Typ des Prinzipals.</span><span class="sxs-lookup"><span data-stu-id="e68aa-139">The type of principal.</span></span>  <span data-ttu-id="e68aa-140">Dies kann entweder "User", "Group" oder "ServicePrincipal" sein.</span><span class="sxs-lookup"><span data-stu-id="e68aa-140">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="e68aa-141">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e68aa-141">resourceDisplayName</span></span>|<span data-ttu-id="e68aa-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e68aa-142">String</span></span>|<span data-ttu-id="e68aa-143">Der Anzeigename der Ressource mit der die Zuordnung hergestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="e68aa-143">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="e68aa-144">resourceId</span><span class="sxs-lookup"><span data-stu-id="e68aa-144">resourceId</span></span>|<span data-ttu-id="e68aa-145">Guid</span><span class="sxs-lookup"><span data-stu-id="e68aa-145">Guid</span></span>|<span data-ttu-id="e68aa-146">Der eindeutige Bezeichner (**Id**) für die Zielressource (Service Principal) für die die Zuordnung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="e68aa-146">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e68aa-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e68aa-147">Relationships</span></span>
<span data-ttu-id="e68aa-148">Keine</span><span class="sxs-lookup"><span data-stu-id="e68aa-148">None</span></span>


## <a name="methods"></a><span data-ttu-id="e68aa-149">Methoden</span><span class="sxs-lookup"><span data-stu-id="e68aa-149">Methods</span></span>

| <span data-ttu-id="e68aa-150">Methode</span><span class="sxs-lookup"><span data-stu-id="e68aa-150">Method</span></span>           | <span data-ttu-id="e68aa-151">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e68aa-151">Return Type</span></span>    |<span data-ttu-id="e68aa-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e68aa-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e68aa-153">Abrufen von appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e68aa-153">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="e68aa-154">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e68aa-154">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="e68aa-155">Lesen Sie Eigenschaften und Beziehungen des AppRoleAssignment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e68aa-155">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="e68aa-156">Update</span><span class="sxs-lookup"><span data-stu-id="e68aa-156">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="e68aa-157">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e68aa-157">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="e68aa-158">AppRoleAssignment-Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="e68aa-158">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="e68aa-159">Delete</span><span class="sxs-lookup"><span data-stu-id="e68aa-159">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="e68aa-160">Keine</span><span class="sxs-lookup"><span data-stu-id="e68aa-160">None</span></span> |<span data-ttu-id="e68aa-161">AppRoleAssignment-Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="e68aa-161">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
