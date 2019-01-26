---
title: Ressourcentyp privilegedApproval
description: Stellt eine Genehmigung, die für die erste in einer Rolle in privilegierten Identity Management angefordert wird.
localization_priority: Normal
ms.openlocfilehash: 03cdba4eee7b031645928b2f512288a18ba18bf8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571017"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="db479-103">Ressourcentyp privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="db479-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db479-104">Stellt eine Genehmigung, die für die erste in einer Rolle in privilegierten Identity Management angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="db479-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="db479-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="db479-105">Methods</span></span>

| <span data-ttu-id="db479-106">Methode</span><span class="sxs-lookup"><span data-stu-id="db479-106">Method</span></span>           | <span data-ttu-id="db479-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="db479-107">Return Type</span></span>    |<span data-ttu-id="db479-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db479-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db479-109">Abrufen von privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="db479-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="db479-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="db479-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="db479-111">Lesen Sie Eigenschaften und Beziehungen des PrivilegedApproval-Objekts.</span><span class="sxs-lookup"><span data-stu-id="db479-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="db479-112">Objekte in der Liste privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="db479-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="db479-113">[PrivilegedApproval](privilegedapproval.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="db479-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="db479-114">Ruft die Auflistung der PrivilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="db479-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="db479-115">Erstellen von privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="db479-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="db479-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="db479-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="db479-117">PrivilegedApproval-Objekt zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="db479-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="db479-118">PrivilegedApproval aktualisieren</span><span class="sxs-lookup"><span data-stu-id="db479-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="db479-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="db479-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="db479-120">PrivilegedApproval-Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="db479-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="db479-121">Myrequests</span><span class="sxs-lookup"><span data-stu-id="db479-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="db479-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="db479-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="db479-123">Get-Anforderungen für das jeweilige Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="db479-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="db479-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="db479-124">Properties</span></span>
| <span data-ttu-id="db479-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="db479-125">Property</span></span>     | <span data-ttu-id="db479-126">Typ</span><span class="sxs-lookup"><span data-stu-id="db479-126">Type</span></span>   |<span data-ttu-id="db479-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db479-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db479-128">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="db479-128">approvalDuration</span></span>|<span data-ttu-id="db479-129">Dauer</span><span class="sxs-lookup"><span data-stu-id="db479-129">Duration</span></span>||
|<span data-ttu-id="db479-130">approvalState</span><span class="sxs-lookup"><span data-stu-id="db479-130">approvalState</span></span>|<span data-ttu-id="db479-131">string</span><span class="sxs-lookup"><span data-stu-id="db479-131">string</span></span>| <span data-ttu-id="db479-132">Mögliche Werte sind: `pending`, `approved`, `denied`, `aborted` und `canceled`.</span><span class="sxs-lookup"><span data-stu-id="db479-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="db479-133">approvalType</span><span class="sxs-lookup"><span data-stu-id="db479-133">approvalType</span></span>|<span data-ttu-id="db479-134">String</span><span class="sxs-lookup"><span data-stu-id="db479-134">String</span></span>||
|<span data-ttu-id="db479-135">approverReason</span><span class="sxs-lookup"><span data-stu-id="db479-135">approverReason</span></span>|<span data-ttu-id="db479-136">String</span><span class="sxs-lookup"><span data-stu-id="db479-136">String</span></span>||
|<span data-ttu-id="db479-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="db479-137">endDateTime</span></span>|<span data-ttu-id="db479-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db479-138">DateTimeOffset</span></span>|<span data-ttu-id="db479-p101">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="db479-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="db479-141">id</span><span class="sxs-lookup"><span data-stu-id="db479-141">id</span></span>|<span data-ttu-id="db479-142">String</span><span class="sxs-lookup"><span data-stu-id="db479-142">String</span></span>| <span data-ttu-id="db479-143">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="db479-143">Read-only.</span></span>|
|<span data-ttu-id="db479-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="db479-144">requestorReason</span></span>|<span data-ttu-id="db479-145">String</span><span class="sxs-lookup"><span data-stu-id="db479-145">String</span></span>||
|<span data-ttu-id="db479-146">roleId</span><span class="sxs-lookup"><span data-stu-id="db479-146">roleId</span></span>|<span data-ttu-id="db479-147">String</span><span class="sxs-lookup"><span data-stu-id="db479-147">String</span></span>||
|<span data-ttu-id="db479-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="db479-148">startDateTime</span></span>|<span data-ttu-id="db479-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db479-149">DateTimeOffset</span></span>|<span data-ttu-id="db479-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="db479-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="db479-152">userId</span><span class="sxs-lookup"><span data-stu-id="db479-152">userId</span></span>|<span data-ttu-id="db479-153">String</span><span class="sxs-lookup"><span data-stu-id="db479-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="db479-154">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="db479-154">Relationships</span></span>
| <span data-ttu-id="db479-155">Beziehung</span><span class="sxs-lookup"><span data-stu-id="db479-155">Relationship</span></span> | <span data-ttu-id="db479-156">Typ</span><span class="sxs-lookup"><span data-stu-id="db479-156">Type</span></span>   |<span data-ttu-id="db479-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db479-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db479-158">roleInfo</span><span class="sxs-lookup"><span data-stu-id="db479-158">roleInfo</span></span>| [<span data-ttu-id="db479-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="db479-159">privilegedRole</span></span>](privilegedrole.md) | <span data-ttu-id="db479-p103">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="db479-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="db479-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="db479-162">request</span></span>| [<span data-ttu-id="db479-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="db479-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md) | <span data-ttu-id="db479-164">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="db479-164">Read-only.</span></span> <span data-ttu-id="db479-165">Die Rolle Zuordnung Anforderung für dieses Objekt Genehmigung</span><span class="sxs-lookup"><span data-stu-id="db479-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db479-166">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="db479-166">JSON representation</span></span>
<span data-ttu-id="db479-167">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="db479-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedApproval"
}-->

```json
{
  "approvalDuration": "string (timestamp)",
  "approvalState": "string",
  "approvalType": "string",
  "approverReason": "String",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "requestorReason": "String",
  "roleId": "String",
  "startDateTime": "String (timestamp)",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedapproval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
